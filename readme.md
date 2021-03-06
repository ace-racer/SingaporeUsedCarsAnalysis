***MongoDb Python API***
Dependencies:
1. Install Mongo DB version 3.6.4 or later
2. Run Mongo DB process and note the port number it is running on
3. install pymongo: pip install pymongo
4. Update the values of MONGO_DB_PORT to the value noted in step 2 above. By default MongoDb runs on port # 27017 and so it need not be changed

API Usage:
1. Insert many car details into the collection: 
See `insert_many_records_sample` method in `MongoDbClient` class
2. Insert single car detail into the collection:
See `insert_single_record_sample` method in `MongoDbClient` class



***Scraping from [Carousell](https://sg.carousell.com/)***
1. Navigate to the robots.txt here: https://sg.carousell.com/robots.txt
2. Get the sitemap URL from the above location. Here it is: https://sg.carousell.com/sitemap.xml
3. Navigate to the sitemap.xml and then search for all product listings with the text "cars"
4. Navigate to each of these XML pages and get the list of the car products in the file
5. Scrape the details of the cars from each of the car product pages

***Configurations***
1. Set the value of ```USE_TEST_URLs``` to ```False``` to execute steps 3 and 4 in the script
2. Set ```LIMIT``` to ```None``` to scrape all the items from the page, else a number that specifies the number of car products which to scrape