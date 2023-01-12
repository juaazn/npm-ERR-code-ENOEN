# npm-ERR code-ENOENT. Does not create a new package.json or install dependencies.

I wanted to start a new package.json with ```npm init -y``` from the windows cmd and the console throws an error. 

**I tried to solve it this way and it didn't work.**
- Remove the npm cache with ```npm cache clean --force```.
- Update to the latest version of npm
- Install the latest version of LTS node.
- Uninstall and install node and it didn't work.



>     C:\Users\ADMIN\Documents\server>npm init -y
>     npm ERR! code ENOENT
>     npm ERR! syscall open
>     npm ERR! path C:\Users\ADMIN\Documents\server\package.json
>     npm ERR! errno -4058
>     npm ERR! enoent ENOENT: no such file or directory, open 'C:\Users\ADMIN\Documents\server\package.json'
>     npm ERR! enoent This is related to npm not being able to find a file.
>     npm ERR! enoent
>     npm ERR! A complete log of this run can be found in:
>     npm ERR!     C:\Users\ADMIN\AppData\Local\npm-cache\_logs\2023-01-12T00_47_42_486Z-debug-0.log


**The npm cache error log**


    > 0 verbose cli C:\Program Files\nodejs\node.exe
    > C:\Users\ADMIN\AppData\Roaming\npm\node_modules\npm\bin\npm-cli.js 1
    > info using npm@9.2.0 2 info using node@v18.13.0 3 timing
    > npm:load:whichnode Completed in 0ms 4 timing config:load:defaults
    > Completed in 2ms 5 timing
    > config:load:file:C:\Users\ADMIN\AppData\Roaming\npm\node_modules\npm\npmrc
    > Completed in 3ms 6 timing config:load:builtin Completed in 3ms 7
    > timing config:load:cli Completed in 2ms 8 timing config:load:env
    > Completed in 0ms 9 timing config:load:project Completed in 3ms 10
    > timing config:load:file:C:\Users\ADMIN\.npmrc Completed in 1ms 11
    > timing config:load:user Completed in 1ms 12 timing
    > config:load:file:C:\Users\ADMIN\AppData\Roaming\npm\etc\npmrc
    > Completed in 0ms 13 timing config:load:global Completed in 1ms 14
    > timing config:load:setEnvs Completed in 1ms 15 timing config:load
    > Completed in 14ms 16 timing npm:load:configload Completed in 14ms 17
    > timing npm:load:mkdirpcache Completed in 0ms 18 timing
    > npm:load:mkdirplogs Completed in 0ms 19 verbose title npm doctor 20
    > verbose argv "doctor" 21 timing npm:load:setTitle Completed in 2ms 22
    > timing config:load:flatten Completed in 3ms 23 timing npm:load:display
    > Completed in 4ms 24 verbose logfile logs-max:10
    > dir:C:\Users\ADMIN\AppData\Local\npm-cache\_logs\2023-01-12T00_58_05_674Z-
    > 25 verbose logfile
    > C:\Users\ADMIN\AppData\Local\npm-cache\_logs\2023-01-12T00_58_05_674Z-debug-0.log
    > 26 timing npm:load:logFile Completed in 15ms 27 timing npm:load:timers
    > Completed in 0ms 28 timing npm:load:configScope Completed in 0ms 29
    > timing npm:load Completed in 37ms 30 silly logfile done cleaning log
    > files 31 timing config:load:flatten Completed in 1ms 32 info Running
    > checkup 33 http fetch GET 200
    > https://registry.npmjs.org/-/ping?write=true 453ms (cache miss) 34
    > http fetch GET 200 https://registry.npmjs.org/npm 261ms (cache miss)
    > 35 timing command:doctor Completed in 4395ms 36 verbose exit 0 37
    > timing npm Completed in 4460ms 38 info ok


I applied the solutions that I mentioned and none of them solved the error. Does anyone know how I could solve it? Since I have not found any method to solve it
