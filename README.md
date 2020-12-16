# Task-of-14-12-2020
const express = require('express')
const app = express();
const port = 8000;

app.use(login)

app.get('/',(req,res)=> {
    res.send("welcome to home page")
    console.log("welcome to home page");
});
app.get('/About',(req,res)=> {
    res.send("Welcom To Our About Page")
    console.log("Welcom To Our About Page");
});
app.get('/registeration',(req,res)=> {
    res.send("Welcom To Our Registeration page")
    console.log("Welcom To Our Registeration page");
});
function login(req,res,next){
    console.log("login sussefull");
    next()
}
app.get('/product',(req,res)=>{
    res.write("toy ")
    console.log("toy");
});
app.get('/pricing',(req,res)=>{
    res.send("taddy bear = 100$ ")
    console.log("taddy bear = 100");
});
app.get('/help',(req,res)=>{
    res.send("how i can help you? ")
    console.log("how i can help you?");
});
app.get('/testimonal',(req,res)=>{
    res.send("more than 1 million people satisfied coustmers !!! ")
    console.log("more than 1 million people satisfied coustmers!!! ");
});
app.get('/programs',(req,res)=>{
    res.send("starter programs ")
    console.log("starter programs");
});
app.get('/blogs',(req,res)=>{
    res.send("more than 100000 blog are cover our products ")
    console.log("more than 100000 blog are cover our products");
});
app.get('/career',(req,res)=>{
    res.send("white coler jobs ")
    console.log("white coler jobs");
});

app.listen(port,()=>{
    console.log('example app lisiting on port $(port)!')
})
