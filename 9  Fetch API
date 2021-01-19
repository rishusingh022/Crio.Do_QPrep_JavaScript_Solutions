//https://www.youtube.com/watch?v=YkFTbnwheVw
//https://www.youtube.com/watch?v=YkFTbnwheVw
const mockFetch = require('./mock-fetch')
const successResponse = [
    {
        'userId': '1',
        "data": 'This looks slick!'
    },
    {
        'userId': '2',
        "data": 'I think this can be improved.'
    },
    {
        'userId': '1',
        "data": 'What kind of improvement?'
    }];
mockFetch('/api/comments', successResponse);
async function getCommentsByUserId(userId) {
    var result;
    arr=[];
    await fetch("/api/comments")
    .then(res => res.json())
    .then(res =>{
        result=res.filter(item => item.userId=userId);
        for(var i=0;i<result.length;i++){
            arr.push(result[i].data);
        }
        arr.sort();
        return arr;
    })
    .catch(err => console.log(err));
}
module.exports = getCommentsByUserId;
console.log(getCommentsByUserId(1));

