# Prerequisites Concerning Datasets
## Installation
* Download [Images](http://vision.stanford.edu/aditya86/ImageNetDogs/images.tar)
and [Annotation](http://vision.stanford.edu/aditya86/ImageNetDogs/annotation.tar) 
from the [**Stanford Dogs Dataset**](http://vision.stanford.edu/aditya86/ImageNetDogs/)
* Put `Annotation` and `Images` into this folder

## File Extension
The extracted data in Annotation folder don't have any `.xml` file extension yet.

Move first to the `Annotation` folder with the `cd` command in your shell

The following command will convert all the files within folders to `.xml`:
* On Windows run:
    ```shell
        for /R %i in (*) do ren "%i" "%~nxi.xml"
    ```
* On MacOS / Linux run:
    ```shell
    find . -type f -exec mv "{}" "{}.xml" \;
    ```
  
Then you are ready to start the project !