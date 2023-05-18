# This document consists of complete basics of mongoose and how to connect with backend serve

# install Mongoose from the command line using npm:
$ npm install mongoose --save

// importing mongoose;
const mongoose = require('mongoose');

main().catch(err => console.log(err));

async function main() {
    await mongoose.connect('mongodb://127.0.0.1:27017/test');
    // use `await mongoose.connect('mongodb://user:password@127.0.0.1:27017/test');` if your database has auth enabled
}

// creating the mongoose schema;
const kittySchema = mongoose.Schema({
    name:String,
    nickname:String,
    age:Number
});

// creating the mongoose model;
const kitten = mongoose.model('kitten', kittySchema);

// this is the mongoose document and the arguments must be same as Schema;
const kittyDocument = new kitten({
    name:'kitten',
    nickname:'kittu',
    age:10,
})

// adding speak functionality;
kittySchema.methods.speak = function speak() {
    const greeting = 'Meow name is ' + kittyDocument.name;
    console.log(greeting);
}

// adding age functionality;
kittySchema.methods.getage = function getage() {
    const myage = kittyDocument.age;
    console.log(`kitty age is ${myage}`);
}

// after any modifications to the schemea, we need to create the new model;
const kit = mongoose.model('kit', kittySchema);

// creating the new Document after added the functions;
const fluffyDocument = new kit({
    name:'kit cat',
    age:10
})

// to save the data to the DataBase we use save() method;
fluffyDocument.save();

// since speak() is a function that we created on kittySchema, we have to call like this;

fluffyDocument.speak(); // output, Meow name is kitten
fluffyDocument.getage(); // output, kitty age is 10
