# LuaEBML

This is a library to read EBML documents.

### Features

Almost all native EBML read features are supported.
- zero data size elements
- EBML element type default values
- element default values
- mandatory elements (which are not always present in the stream)
- unknown size elements (Master element)
- reading an entire Master element
- damaged data
- option to allow Dummy elements

The only feature that is not supported is external global elements. Only the EBML global elements, Void and CRC-32 are supported.

No data is read for the Void element, it is simply skipped.

### Lua versions

LuaEBML has some sort of "compiler switches" to still support older Lua versions that don't do bit operations.
Older versions means Lua5.1, Lua5.2 and LuaJIT. Since Lua5.3 bit operations are supported.