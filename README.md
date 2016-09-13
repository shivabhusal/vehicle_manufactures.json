# Vehicle Manufactures List
This repo consists of all the active vehicle manufacturers in the World.
> **Note**: Only consists of active vehicle vendors. No Defunct are listed here.

List is in `JSON` format and separated/organized by `Country` name

## Parsing data in Ruby
- [Copy the file](/vehicle_vendor_list.json) `vehicle_vendor_list.json` to your working directory
- From the loader ruby file [it may be `seeds.rb`] for `Rails` Projects
 ```ruby
 require 'json'
 
 file = File.expand_path('../vehicle_vendor_list.json', __FILE__)
 vehicle_data = data = JSON.parse(File.read(file))
 
 # Output
 => [{"Argentina"=>
    ["Alcre",
     "Anasagasti",
     "Arbus",
     "Autoar",
     "Cametal",
     "Crespi",
     "De Carlo",
     "Dinarg",
     "Dinborg",
     "El Detalle",
     "Eniak",
     ...

 ```

# Contribution
Please feel free to fork this project and send pull requests. Help me keep this repo up to date.

# Sources
This database is extracted out [from Wikipedia](https://en.wikipedia.org/wiki/List_of_automobile_manufacturers)
