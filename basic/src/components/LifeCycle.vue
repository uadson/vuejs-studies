<template>
    <div>
        <h3>Life Cycle Hook</h3>
        <p> This is a Life Cycle Hook's example:</p><br>
            <p>A data will be returned: <b>{{ data }}</b></p><br>
            <code>
                <pre>
                script
                    export default {
                        name: 'LifeCycle',

                        data() {
                            return {
                                <b><u>data: "Something"</u></b>       
                            }
                        }
                    }
                script
                </pre>
            </code>
        <p>After that, with created() method:</p><br>
            <p>A data will be returned: <b>{{ data }}</b></p><br>
            <code>
                <pre>
                script
                    export default {
                        name: 'LifeCycle',

                        data() {
                            return {
                                data: "Something"     
                            }
                        },
                        created() {
                            <b><u>this.data = "Some Data"</u></b>
                        }
                    }
                script
                </pre>
            </code>
        <p>Next example, with mounted() method:</p><br>
            <p>A data will be returned: <b>{{ data }}</b></p><br>
            <code>
                <pre>
                script
                    export default {
                        name: 'LifeCycle',

                        data() {
                            return {
                                data: "Something"     
                            }
                        },
                        created() {
                            this.data = "Some Data"
                        },
                        mounted() {
                            <b><u>this.data = "Another Data"</u></b>
                        }
                    }
                script
                </pre>
            </code>
    </div>
</template>

<script>
    export default {
        name: 'LifeCycle',

        data() {
            return {
                data: "Something"       
            }
        },
        created() {
            setTimeout(() => {
                this.data = "Some Data"
            }, 3000);
        },
        mounted() {
            setTimeout(() => {
                this.data = "Another Data"
            }, 5000);
        }
    }
</script>