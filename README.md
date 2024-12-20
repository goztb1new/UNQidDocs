# Unique ID Module Documentation

Requiring Module:
```
local UNQID = require(PATHTOMODULE)
```

Creating Shared globals:
```
UNQID.GenUID(ToShare, UID:String)
local ExampleBool = UNQID.GenUID(true, "BooleanTestTrue") -- Example Boolean
local ExampleString = UNQID.GenUID("Test UNQID STRING", "StringTextTest") -- Example Text
local ExampleInstance = UNQID.GenUID(workspace["UNQ TESTING"].Part, "InstanceTest") -- Example Instance
```

Recieving UIDS in order to Recive Info Table: 
```
local BoolTest = UNQID.ReciveUID("BooleanTestTrue")
local StringTest = UNQID.ReciveUID("StringTextTest")
local InstanceTest = UNQID.ReciveUID("InstanceTest")
```

Printing Out: MAKE SURE YOU ARE TRYING TO RECIVE THEM AFTER YOU GENERATED THEM, OTHERWISE IT WILL RETURN nil
```
print(UNQID.ReciveUNQTable(BoolTest).ItemObject)
print(UNQID.ReciveUNQTable(StringTest).ItemObject)
print(UNQID.ReciveUNQTable(InstanceTest).ItemObject)
```
