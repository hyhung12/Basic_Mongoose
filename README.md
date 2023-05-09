# Basic_Mongoose

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
