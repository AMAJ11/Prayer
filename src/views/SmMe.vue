<template>
    <div class="sm mt-15">
        <v-container>
            <v-row>
                <v-col>
                    <v-card class="cr" style="text-align: center;padding: 30px;padding-bottom:0">
                        <v-card-title class="text-primary" style="font-size:40px !important">عمّار أبو
                            جيب</v-card-title>
                        <v-card-text class="text-h5"> Front-End Developer with <span class="text-red">Vue
                                js</span> framework </v-card-text>
                        <p class="text-button"> <span class="text-success">From</span> Syria Damascus ❤️</p>
                        <v-alert color="primary" variant="tonal">Student Of ITE in Damascus university</v-alert>
                        <v-card-actions class="mt-8"
                            style="text-align: center;display:flex;align-items:center;justify-content: center;">
                            <div>
                                <a href="https://www.facebook.com/ammar.aj.927"><v-btn class="bt" color="success">
                                        <v-icon size="x-large" style="font-size:38px !important"> mdi-facebook </v-icon>
                                    </v-btn></a>
                                <a href="https://www.instagram.com/ammar.aj.927/"> <v-btn class="bt" color="success">
                                        <v-icon size="x-large" style="font-size:38px !important">
                                            mdi-instagram </v-icon>
                                    </v-btn></a>
                                <a href="https://github.com/AMAJ11/"> <v-btn class="bt" color="success"> <v-icon
                                            size="x-large" style="font-size:38px !important"> mdi-github </v-icon>
                                    </v-btn></a>
                                <a href="https://www.linkedin.com/in/ammar-amaj-606579202/"> <v-btn class="bt"
                                        color="success"> <v-icon size="x-large" style="font-size:38px !important">
                                            mdi-linkedin </v-icon> </v-btn></a>
                                <a href="https://api.whatsapp.com/send/?phone=963937379312"> <v-btn to="" class="bt"
                                        color="success"> <v-icon size="x-large" style="font-size:38px !important">
                                            mdi-whatsapp </v-icon> </v-btn></a>
                            </div>
                        </v-card-actions>
                    </v-card> </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<style scoped>
@media (max-width:350px) {
    .cr {
        padding: 10px 0 !important
    }
}

.bt {
    transition: .2s
}

.bt:hover {
    translate: 0 -8px;
}
</style>
<script>
export default {

}
</script>