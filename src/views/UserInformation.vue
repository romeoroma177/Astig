<template>
   
    <div>
         <Head />
        <div class="mx-auto form-container">
            <h2>Create Account</h2>
            <p>Fill up user details </p>
            <form>
                <div action="" class="user-information">
                    <input type="text" class="form-control" name="idnumber" id="" placeholder="First Name">
                    <input type="text" class="form-control" name="password" id="" placeholder="Middle Name">
                    <input type="text" class="form-control" name="r-password" id="" placeholder="Last Name">
                    <input type="text" class="form-control" name="r-password" id="" placeholder="Prefix">
                    <input type="text" class="form-control" name="r-password" id="" placeholder="Suffix">
                    <input type="text" class="form-control" name="r-password" id="" placeholder="Office">
                    <input type="text" class="form-control" name="r-password" id="" placeholder="Service">
                    <input type="text" class="form-control" name="r-password" id="" placeholder="Division">
                </div>
                <input type="submit" @click.prevent="proceedQuery()" class="btn btn-outline-primary col-xl-12" id="next" value="Create">
                <input type="submit" @click.prevent="cancelQuery()" class="btn btn-outline-danger col-xl-12" id="next" value="Cancel">
            </form>
        </div>
    </div>
</template>

<script>
import Head from './layout/Head'

export default {
    name: 'UserInformation',
    methods: {
         proceedQuery() {
            this.$router.push('/login')
        },
        cancelQuery() {
            this.$router.push('/register')
        }
    }, 
    components: {
        Head
    }
}
</script>

<style scoped>
.user-information {
    height: 200px;
    overflow: scroll;
}

</style>>
