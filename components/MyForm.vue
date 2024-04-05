<template>
    <v-app>
        <v-container>
            <v-form>
                <div class="text-uppercase text-h5 text-center">
                    HỒ SƠ KHÁM BỆNH / MEDICAL RECORD / 진료 기록
                </div>
                <v-row no-gutters>
                    <v-col cols="2">
                        <v-sheet class="pa-2 ma-2">
                            <div></div>
                        </v-sheet>
                    </v-col>

                    <v-col cols="10">
                        <v-sheet class="pa-2 ma-2">
                            <label>Mã số y tế / Identification (I.D) number /의료 번호 :</label>
                            <v-text-field v-model="mayte"></v-text-field>

                            <label>1. Họ và tên / Full name /성함:</label>
                            <v-text-field  v-model="hoten"></v-text-field>


                            <div style="display: flex; align-items: center; ">
                                <label style="padding-bottom: 22px;">2. Giới tính/ Gender /성별:</label>
                                <v-checkbox label="Nam/ Male (남성)" v-model="gioitinhnam"></v-checkbox>
                                <v-checkbox label="Nữ/ Female(여성)" v-model="gioitinhnu"></v-checkbox>
                            </div>

                            <label>3. Ngày tháng năm sinh / Birthday /생년월일:</label>
                            <v-text-field  v-model="ngaysinh"></v-text-field>

                            <label>4. Số CCCD/ National I.D number/주민등록번:</label>
                            <v-text-field  v-mode="cmnd"></v-text-field>

                            <label>5. Địa chỉ / Address/주소 :</label>
                            <v-text-field  v-model="diachi"></v-text-field>

                            <label>6. Điện thoại/ Mobile phone /휴대폰:</label>
                            <v-text-field  v-model="sodienthoai"></v-text-field>

                            <v-btn>Submit</v-btn>
                        </v-sheet>
                    </v-col>
                </v-row>
            </v-form>
        </v-container>
    </v-app>
</template>

<script>
export default {
    data() {
        return {
            mayte: '',
            hoten: '',
            gioitinhnam: true,
            gioitinhnu: false,
            ngaysinh: '',
            cmnd: '',
            diachi: '',
            sodienthoai: '',
        }
    },
    methods: {},
}
</script>

<style></style>
