<template>
    <main class="container-lg">
        <header>
            <h4>INFORMAÇÕES DA EMPRESA</h4>
        </header>

        <form class="cadastro" @submit.prevent="prevent">
            <section class="d-flex gap-3">
                <div>
                    <div class="text-start">Logo da empresa</div>
                    <input type="file" class="form-control" id="logo" name="logo" placeholder="Opcional">
                </div>

                <div>
                    <div class="text-start">Nome da sua empresa</div>
                    <input type="text" class="form-control" id="nome_estabelecimneto" name="nome_estabelecimento" required>
                </div>

                <div>
                    <div class="text-start">Ramo</div>
                    <input type="text" class="form-control" id="ramo" name="ramo" required>
                </div>

                <div>
                    <div class="text-start">Horário de funcionamento</div>
                    <input type="date" class="form-control" id="hora_funci" name="hora_funci" required>
                </div>
            </section>

            <button class="btn bg-secondary text-white">Registrar dados</button>
        </form>
    </main>
</template>

<script>
    export default {
        name:'CadastroView',
        data() {
            return {
                
            }
        },

        methods: {
            prevent(){
                alert("Empresa cadastrada")
            }
        },
    }
</script>

<style scoped>
label{
    margin-left: 0px;
}
</style>