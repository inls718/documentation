Various notes on how the GRC file seems to function, as well as ideas for how it can be used by various teams going forward.

This file is created for the reference of the developers, aka US.

- GRC file contains XML
- tags define the properties associated with a single block. Includes parameters, assigned, key-value pairs, coordinates for positioning 
- on flow chart, linked blocks, etc.
- lines between blocks are stored in the file as a separate object, defined by the tags
- holds start block and block only
- does NOT seem to hold any information on the actual signal, just how the blocks have been set up to process the signal
- GRC file only holds the CURRENT state of the flow chart, does not store information for any blocks/connections that are present
- if we want starting parameters or presets, we can do that by defining values or whole GRC files
- experimental configurations can be saved as uniquely ID'd GRC files
- we want to know where the origin point of the flow chart is, in case we want to be able to position items on it upon loading (positions stored as x-y coordinates, not clear where (0,0) is located)
