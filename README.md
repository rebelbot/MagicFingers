# MagicFingers
For RE project on single-use, assay-based dispoable COVID test cartridges. The name of this project is left off the record.

## Usage
Normal usage of the test system includes creating an user account, charging a Bluetooth-based test unit that prepares a test sample.
1. Once the user is logged into their app on a smart phone, a new test is started.
2. A cartridge is inserted into the tester and its contents is heated up.
3. A sample is collect from the nose (yes the video is amusing) and inserted into the pre-heated cartridge already inside the tester which triggers the test to start.
4. 25 minutes later, **boom** a result is issued.

## Teardown
Using a dremel remove the long edge along the sample stick and remove most of the outter cover to reveal the pcb and microfluidics assembly. A small plastic device works with the plastic on the clear part of the assembly, plastic enclosure, and sample collection stick to not only start the test but also lock the collection stick in place. In theory, this should protect the user from accessing the chemical assays.

![front of PCB](https://github.com/rebelbot/TingleFinger/blob/main/pictures/top_pcb.jpg)
![back of PCB](https://github.com/rebelbot/TingleFinger/blob/main/pictures/back_pcb.jpg)
![removed IC](https://github.com/rebelbot/TingleFinger/blob/main/pictures/removed_IC.jpg)
Stuffed on the PCB are a handful of passives and a clearly marked [ST M240C EEPROM](https://www.st.com/resource/en/datasheet/m24c04-f.pdf). Since the plastic microfluidics are over the interesting parts of the PCB and I like keeping the rest of my fingers tingle-free, I opted to not disturb it further and just dremels out the IC. I then desoldered it and plopped it into my TL866 reader to get the data. 
![Quick snap of data](https://github.com/rebelbot/TingleFinger/blob/main/pictures/extracted_data_setup.jpg)

## TODOs
[] Process remaining cartridges and determine if they are different or share the same info.
