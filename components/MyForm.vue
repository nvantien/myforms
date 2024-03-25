<script>
  export default {
    data: () => ({
      model: 'Âm tính (Negative)',
    }),
  }
</script>

<template>
    <VApp>
        <VContainer>
            <div class="text-uppercase text-h5 text-center">
                HỒ SƠ KHÁM BỆNH / MEDICAL RECORD / 진료 기록
            </div>
            <VRow no-gutters>
                <VCol cols="2">
                    <VSheet class="pa-2 ma-2">
                        <v-img :width="400" height="150" aspect-ratio="4/3" cover
                            src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"></v-img>
                    </VSheet>
                </VCol>
                <VCol>
                    <VSheet class="pa-2 ma-2">
                        <table>
                            <tr>
                                <td>Mã số y tế / Identification (I.D) number /의료 번호 :</td>
                                <td><v-text-field /></td>
                            </tr>
                            <tr>
                                <td>1. Họ và tên / Full name /성함:</td>
                                <td><v-text-field /></td>
                            </tr>
                            <tr>
                                <td>2. Giới tính/ Gender /성별:</td>
                                <td>
                                    <v-checkbox label="Nam/ Male (남성)"></v-checkbox>
                                </td>
                                <td>
                                    <v-checkbox label="Nữ/ Female(여성)"></v-checkbox>
                                </td>
                            </tr>
                            <tr>
                                <td>3. Ngày tháng năm sinh / Birthday /생년월일:</td>
                                <td>
                                    <v-text-field /> <v-date-picker style="display: none" />
                                </td>
                            </tr>
                            <tr>
                                <td>4. Số CCCD/ National I.D number/주민등록번:</td>
                                <td><v-text-field /></td>
                            </tr>
                            <tr>
                                <td>5. Địa chỉ / Address/주소 :</td>
                                <td><v-text-field /></td>
                            </tr>
                            <tr>
                                <td>6. Điện thoại/ Mobile phone /휴대폰:</td>
                                <td><v-text-field /></td>
                            </tr>
                        </table>
                    </VSheet>
                </VCol>
            </VRow>
        </VContainer>
        <VContainer>
            <div class="text-uppercase text-h5">
                I. KHÁM THỂ LỰC / PHYSICAL EXAMINATION / 신체 검사
            </div>
            <VRow no-gutters>
                <VCol cols="12">
                    <table>
                        <tr>
                            <td>Chiều cao / Height /키:</td>
                            <td><v-text-field /></td>
                            <td>cm - Cân nặng / Weight /몸무게:</td>
                            <td><v-text-field /></td>
                            <td>Kg - Chỉ số BMI / BMI 지수:</td>
                            <td><v-text-field /></td>
                        </tr>
                    </table>
                    <table>
                        <tr>
                            <td>Mạch /Pulse rate / 맥박:</td>
                            <td><v-text-field /></td>
                            <td>lần/phút - Huyết áp / Blood Pressure / 혈압:</td>
                            <td><v-text-field /></td>
                            <td>/</td>
                            <td><v-text-field /></td>
                            <td>mmHg</td>
                        </tr>
                    </table>
                </VCol>
            </VRow>
        </VContainer>
        <VContainer>
            <div class="text-uppercase text-h5">II. KHÁM LÂM SÀNG / CLINICAL EXAMINATION / 임상 검사</div>

        </VContainer>
        <VContainer>
            <div class="text-uppercase text-h5">III . KHÁM CẬN LÂM SÀNG / PARACLINICAL EXAMINATION / 유방검사 </div>
            <table>
                <tr>
                    <td>
                        Xét nghiệm / Lab Test /검사
                    </td>
                    <td style="width: fit-content;">Kết quả / Results /결과</td>
                    <td>Chỉ số Bình thường / Reference Range /정상 범위 </td>
                </tr>
                <tr>
                    <td>
                        Syphilis / 매독
                    </td>
                    <td>
                    <td><v-text-field v-model="model" hide-details="auto" clearable>
                    </v-text-field>
                    </td>
                    S/CO < 1
                    </td>
                    <td>

                    </td>
                </tr>
            </table>

        </VContainer>
    </VApp>
</template>

<style>
.table-ls {
    border: 1px solid #000000;
}

.table-ls th {
    border-top: 1px solid #e6e6e6;
}

.table-ls th+th {
    border-left: 1px solid #e6e6e6;
}

.table-ls td+td {
    border-left: 1px solid #e6e6e6;
}
</style>