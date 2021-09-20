 <template>
    <form action="" method="POST">
        <h1>Survey</h1>
        <p>Name: <input type="text" v-model="name" ></p>
        <p>Location: 
            <select v-model="locationId">
                <option value="1">Seattle</option>
                <option value="2">Minneapolis</option>
                <option value="3">Dallas</option>
                <option value="4">Richmond</option>
            </select>
        </p>
        <p>Category: 
            <select v-model="languageId" >
                <option value="1">Javascript</option>
                <option value="2">Python</option>
                <option value="3">Java</option>
                <option value="4">C#</option>
            </select>
        </p>
        <p>Description: <br /><textarea v-model="comments" ></textarea></p>
        <p><input type="submit" value="Add Item"></p>
    </form>
</template>

<script>
export default {
    name: "FormPractice",
    data: function() {
        return {
            name: '',
            locationId: 1,
            languageId: 1,
            comments: ''
        };
    }
}

</script>
<style scoped>
    p {
        margin: auto;
        margin-top: 2%;
        width: 30%;
        display: flex;
        justify-content: space-between;
    }
    form {
        border: 1px solid black;
        padding: 1%;
    }
    input[type=submit] {
        margin: auto;
    }

</style>