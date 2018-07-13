# Simple Database

## Project Description
A simple object database that stores and retrieves objects from the file system.

## Developer
Requires Node v10 or later.

### how to get started
* Fork repository, clone locally, navigate to repository directory,
* Download all the files with `npm i`,
* To test, run `npm test`. 

### how to use API
* `.save(<objectToSave>)` will stringify and then save the object to a JSON file with a unique id.
    ```js
    store.save({ name: Mickey Mouse });
    ```
* `.get(<id>)` will find the JSON file with the corresponding ID and get a parsed object.
    ```js
    store.get(cat._id)
    ```
* `.remove(<id>)` will find the JSON file with the corresponding ID and delete it, returning `true` if it was successful and `false` if it didn't find the file.
    ```js
    store.remove(cat._id)
    ```
* `.getAll()` will get an array of all the objects in the directory, or an empty array if it's empty.
    ```js
    store.getAll();
    ```

## Contributor
Mariah Adams

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgment 
Forked from [alchemy-fullstack-js-summer-2018/simple-database](https://github.com/alchemy-fullstack-js-summer-2018/simple-database)