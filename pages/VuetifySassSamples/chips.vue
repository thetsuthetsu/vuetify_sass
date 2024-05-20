<template>
    <div>
        <v-container>
            <v-row>
                class selector (Sass variables)
            </v-row>
            <v-row>
                <div class="sass_color1">
                    <v-chip>
                        $custom_chip_color1
                    </v-chip>
                </div>
                <div class="sass_color2">
                    <v-chip>
                        $custom_chip_color1
                    </v-chip>
                </div>
            </v-row>
            <v-row>
                <v-divider/>
            </v-row>
            <v-row>v-chip color property (Vuetify Default Lite Theme Colors)</v-row>
            <v-row>
                <v-col>
                    <v-chip>
                        Default
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="surface" variant="flat">
                        Surface
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="primary">
                        Primary
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="secondary">
                        Secondary
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="error">
                        Error
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="info">
                        Info
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="success">
                        Success
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="warning">
                        Warning
                    </v-chip>
                </v-col>
            </v-row>                
            <v-row>
                <v-divider/>
            </v-row>
            <v-row>v-chip color property</v-row>
            <v-row>
                <v-col>
                    <v-chip color="red">
                        Red
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="red-darken-4">
                        red-darken-4
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="blue">
                        Blue
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="green">
                        Green
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="yellow">
                        Yellow
                    </v-chip>
                </v-col>                
                <v-col>
                    <v-chip color="#FF8800">
                        #FF8800
                    </v-chip>
                </v-col>                
            </v-row>
            <v-row>
                <v-divider/>
            </v-row>
            <v-row>v-chip color property (reactive)</v-row>
            <v-row>
                <v-col>
                    <v-chip :color="color1">
                        Color1
                    </v-chip>
                    <v-color-picker v-model="color1"/>
                </v-col>                
                <v-col>
                    <v-chip :color="color2">
                        Color2
                    </v-chip>
                    <v-color-picker v-model="color2"/>
                </v-col>                
                <v-col>
                    <v-chip :color="color3">
                        Color3
                    </v-chip>
                    <v-color-picker v-model="color3"/>
                </v-col>                
            </v-row>
        </v-container>
    </div>
</template>
<script setup>
    import { ref } from "vue";
    const color1 = ref('#888888')
    const color2 = ref('#888888')
    const color3 = ref('#888888')
</script>
<style lang="scss">
@import "~/assets/variables.scss";
.sass_color1 {
    color: $custom_chip_color1;
}
.sass_color2 {
    color: $custom_chip_color2;
}
</style>