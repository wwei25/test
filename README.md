# Display function call list
lua_rawget
  |--index2addr
  |--luaH_get
    |--luaH_getshortstr
    |--luaH_getint
    |--luaV_tointeger
      |--luaO_str2num
        |--l_str2int
          |--isneg
          |--luaO_hexavalue
        |--l_str2d
          |--l_str2dloc
    |--getgeneric
      |--mainposition
        |--l_hashfloat
        |--luaS_hashlongstr
          |--luaS_hash
lua_rawget
|-$$index2addr
|-$$luaH_get
|-|-$$luaH_getshortstr
|-|-$$luaH_getint
|-|-$$luaV_tointeger
|-|-|-$$luaO_str2num
|-|-|-|-$$l_str2int
|-|-|-|-|-$$isneg
|-|-|-|-|-$$luaO_hexavalue
|-|-|-|-$$l_str2d
|-|-|-|-|-$$l_str2dloc
|-|-$$getgeneric
|-|-|-$$mainposition
|-|-|-|-$$l_hashfloat
|-|-|-|-$$luaS_hashlongstr
|-|-|-|-|-$$luaS_hash
