# Postman---JSON---Cozumleme

****JSON ÇÖZÜMLEME****

pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

let response=pm.response.json();
console.log(response.prefs.permissionLevel);
console.log(response.prefs.voting);
console.log(response.prefs.invitations);

let a="udemy"   
let b="udemy"
pm.test("a ve b eşit", function () {
    pm.expect(a).is.eql(b); 
});

let c="udemy" 
let d="Udemy"
pm.test("a ve b eşit değil", function () {
    pm.expect(a).is.not.eql(b);
});
