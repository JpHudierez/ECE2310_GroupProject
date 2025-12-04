# Group Project ECE 2310

# Part 1
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

# Part 2 
UML Diagram
<img src="https://media.discordapp.net/attachments/1443418398401888357/1446017427774115910/7de7374b-02d2-4f7d-a5e9-c03ff43854a7.png?ex=6932742c&is=693122ac&hm=2d8b324a1b128008dcf60a3d0a81e0b7dbb4520b0f83968be7cf28d7d6a443b2&=&format=webp&quality=lossless&width=804&height=920" title=Output2 height = 812 width = 709>

Objectives 