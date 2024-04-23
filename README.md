# Espresso-Emporium-Coffee-backend
## crud operation: 

### 1. create:
(i) send document to the server.
(ii) create an api to get the document from client side.
(iii) upload to the mongodb.

### 2. read:
(i) read data with bellow code
```
app.get('/coffee', async (req, res) => {
            const cursor = await coffeeCollection.find({}).toArray();
            // console.log(cursor);
            res.send(cursor)
})
```
### 3. delete:
(i) jake delete korbo take age pakrao kori.[ekti function create kori then delete btn e click korai jake delete korbo tar data server e send kori]
(ii) server e ekti route create kori. jekha theke boli ka bakrake catch kori.
(iii) mongodb theke delete kori
```
const query = { title: "Annie Hall" };
const result = await movies.deleteOne(query);
```
### 4. Update: 
(i) ami age jake update korbo take dhorbo. 
(ii) update btn e click kora hole update page e move korbo and specific item ke load korbo(specific item ke load korar jonno ekti api create korte hobe)
(iii) fetch data of the item which need to be updated and set data as default valus of the input fields.
(iv) colect updated data and send to the server.
(v) recieve data from client side and send to mongodb