## Basic_Mongoose

### Step 1: Connect to database
```
const uri = 'mongodb+srv://hyhung12:babykute@cluster0.ijfrnwn.mongodb.net/mongo_test';

mongoose.connect(uri)
  .then(() => console.log('Connected to MongoDB'))
  .catch(err => console.error('Error connecting to MongoDB', err));
  
// mongoose.connect('mongodb+srv://hyhung12:babykute@cluster0.ijfrnwn.mongodb.net/mongo_test');
```
### Step 2: Define schema (optional)
```
// const weatherSchema = new mongoose.Schema();
const abcd = mongoose.model('test12', {});
const abcd = mongoose.model('test12', mongoose.Schema());
```
### Step 3: Retrieve data
```
abcd.find()
.then(res => {
    console.log(res);
})
.catch(error => {console.log(error);})
```

## Basic_Prisma
|Command|Description|
|-|-|
|npm install prisma --save-dev|Start prisma project|
|npx prisma init||
|npm install @prisma/client||
|npx prisma db pull --force| Load collections & check if connection ok|
|npx prisma generate|When schema is updated|

```
model est12 {
  id    String @id @default(auto()) @map("_id") @db.ObjectId
  Age   String
  Level String
  Name  String
}
```
### GET
```
var data = await prisma.test12.findMany({
where: {},
include: {}
})
```
### POST
var data = await prisma.test12.create({
  data: {
  },
  })
### DELETE






