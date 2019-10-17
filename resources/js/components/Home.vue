<script>
    export default {
        name: 'Home',
        props: {
            msg: String
        },
        data: function() {
            return {
                obj: {
                    name : 'Object name',
                    features: 'Object features',
                    category: 'Object category'
                }
            }
        },
        mounted() {
        }
    }
</script>

<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-12">
                <div class="card">
                    <div class="card-header">{{msg}}</div>

                    <div class="card-body">
                        
                        <h4>Details:</h4>
                        <ul>
                            <li><b>Name: </b>{{this.obj.name}}</li>
                            <li><b>Features: </b>{{this.obj.features}}</li>
                            <li><b>Category: </b>{{this.obj.category}}</li>
                        </ul>
                    </div>

                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    ul {
        list-style: none;
    }
</style>