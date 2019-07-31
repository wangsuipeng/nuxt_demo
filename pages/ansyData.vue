<template>
    <div>
        <h1>姓名：{{info.name}}</h1>
        <h2>年龄：{{info.age}}</h2>
        <h2>兴趣：{{info.interest}}</h2>
        <img src="~static/xiyangyang.jpg" alt="">
    </div>
</template>
<script>
import axios from "axios";
export default {
    data() {
        return {};
    },
    asyncData() {
        return axios.get("https://api.myjson.com/bins/8gdmr")
            .then(result => {
                return { info: result.data };
            })
            .catch(err => { 
                console.log(err)
            });
    },
    async asyncData(){
        let {data}=await axios.get('https://api.myjson.com/bins/8gdmr')
        return {info: data}
    }
};
</script>
