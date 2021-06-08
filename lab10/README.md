# Lab 10

## Student information
* Full name: Xinning Dong
* E-mail: xdong009@ucr.edu
* UCR NetID: xdong009
* Student ID: 861306702

## Answers

* (Q1). mongoimport --db lab10 --collection contacts --file contacts.json --jsonArray<br />
* (Q2).db.contacts.find().sort({Name:1});<br />
* (Q3).db.contacts.find({},{_id:1,Name:1}).sort({Name:-1});<br />
* (Q4).Yes, it is case-sensitive. If we change the first "Name" to "name" in previous query, we can only see id.<br />
* (Q5).db.contacts.find({},{_id:0,Name:1}).sort({Name:-1});<br />
* (Q6).Yes it does.<br />
* (Q7).It should be at top because it is object and in descending order.<br />
* (Q8).Use "David". It is between "Hayes Weaver" and "Craft Parks".<br />
* (Q9).Use "Bark". It is between "Aimee Mcintosh" and "Cooke Schroeder".<br />
* (Q10).db.contacts.createIndex({"Name":1}); Yes it is able to do so.<br />

