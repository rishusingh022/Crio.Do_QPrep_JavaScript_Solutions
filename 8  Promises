//https://www.youtube.com/watch?v=RvYYCGs45L4
//https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise
function getLastNames(firstName, people) {
    return new Promise(( resolve, reject )=>{
        var arr = [];
        typeof people;

        people.map((item)=>{
            if (firstName == item.firstName ){
                arr.push(item.lastName)
            }
        })

        if (arr.length == 0 ){
            reject("Invalid")
        }else {
            resolve(arr.sort())
        }
    })
}

module.exports = getLastNames;
console.log(getLastNames(firstName = 'David',

people = [

        {

            firstName: 'David',

            lastName: 'Dobrick'

        },

        {

            firstName: 'David',

            lastName: 'Beckham'

        },

        {

            firstName: 'Chris',

            lastName: 'Lee'

        },

        {

            firstName: 'James',

            lastName: 'Bond'

        },

    ]
));