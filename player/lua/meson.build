lua_files = ['defaults.lua', 'assdraw.lua', 'options.lua', 'osc.lua',
             'ytdl_hook.lua', 'stats.lua', 'console.lua', 'auto_profiles.lua',
             'input.lua', 'fzy.lua', 'select.lua', 'positioning.lua',
             'commands.lua']
foreach file: lua_files
    lua_file = custom_target(file,
        input: file,
        output: file + '.inc',
        command: [file2string, '@INPUT@', '@OUTPUT@', '@SOURCE_ROOT@'],
    )
    sources += lua_file
endforeach
