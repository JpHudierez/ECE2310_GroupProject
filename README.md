# Group Project ECE 2310

<img src="https://media.discordapp.net/attachments/1443418398401888357/1443463371721801900/image.png?ex=69292986&is=6927d806&hm=17fd133f479b7c9f30c8757472e99ca1ccf2699c5a266a382cea9698f45f6993&=&format=webp&quality=lossless&width=1094&height=731" title=Output height=875 width=585 alt=output>

# Object Explanation
CSV Reader both reads files then outputs the file contents. It lists all the info from the telemetry file in list form.

SensorData takes the data from lists, and retrieves and specifies what the values' functions are.

Hub is the center of the system. It gets the data back and modifies the data (specifically the temperature) to be in Celsius. It also calls upon DataOutput to output the data and CSVReader to read data.

DataOutput writes the finalized data. 

# Relationships
Hub manages SensorData : Hub stores and controls a list of SensorData objects.

Hub uses CSVReader: Hub relies on CSVReader to load data from CSV files.

CSVReader creates SensorData: CSVReader builds SensorData objects from each CSV row.

Hub uses DataOutput: Hub sends its processed data to DataOutput to generate the final output.