# Multi CardServer R63 E0 

Multics is cardserver proxy to share your subscription card at home
It's based on [box/spout](https://github.com/box/spout).

Author: [Evileyes]

Modified by [Messi89](https://github.com/messi89) to :

- Support E0 (Csat & TNT)
- Ecm length increased
- Freeze on full cws change fixed (tags 80/81)
- Autoreferesh on Home tab

[Compilation](#compilation)  
[How to](#how-to)  
[Tested on](#tested-on)  
[Todo](#todo)  
[Thanks to](#thanks-to)  

## Compilation 
use the shell script
```
$ ./makeall.sh 
```


## How to

```
Copy multics.e0 (folder x64 or x86) and multics.e0.cfg (folder config) to /var/multics/
Chmod -R 775 /var/multics/
Start multics : /var/multics/multics.e0 -b or /var/multics/multics.e0 -b -C /config_path
```  

## Tested on

- Oscam r11283 (Cardreader)-> Multics R63 E0 -> Oscam r11283 (Client dvbapi)
- All readers on CCcam protocol

## Todo

- Cache compatibility
- CSS style support
- Fix HTTP bug


## Thanks to

Evileyes, Constance, Pat