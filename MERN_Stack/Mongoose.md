## This document consists of complete basics of mongoose and how to connect with backend server.
> Starting with installation.

### install Mongoose from the command line using npm:

#### npm install mongoose --save


> we can start using mongoose in the vs code.

const mongoose = require('mongoose');

main().catch(err => console.log(err));

async function main() { <br>
     await mongoose.connect('mongodb://127.0.0.1:27017/test'); <br>
}

### creating the mongoose schema; <br>

         const kittySchema = mongoose.Schema({ 
                name:String,  
                nickname:String, 
                age:Number 
            }); 

### creating the mongoose model; <br>

           const kitten = mongoose.model('kitten', kittySchema);   
           
### creating mongoose document;
> this is the mongoose document and the arguments must be same as Schema; <br>

            const kittyDocument = new kitten({
                name:'kitten', 
                nickname:'kittu', 
                age:10,
            }) 
            
### adding methods / functions to our Schema;

// adding speak functionality; <br>

        kittySchema.methods.speak = function speak() {
            const greeting = 'Meow name is ' + kittyDocument.name;
            console.log(greeting);
        }

// adding age functionality; <br>

        kittySchema.methods.getage = function getage() {
            const myage = kittyDocument.age;
            console.log(`kitty age is ${myage}`);
        }

// after any modifications to the schemea, we need to create the new model; <br>

        const kit = mongoose.model('kit', kittySchema); 

// creating the new Document after added the functions; <br>

        const fluffyDocument = new kit({
            name:'kit cat',
            age:10
        })

// to save the data to the DataBase we use save() method; <br>
fluffyDocument.save(); <br>

// since speak() is a function that we created, so have to call like this; <br>

fluffyDocument.speak(); // output, Meow name is kitten <br>
fluffyDocument.getage(); // output, kitty age is 10 <br>
