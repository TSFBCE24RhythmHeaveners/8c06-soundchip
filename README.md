# The 8C06 Sound Chip
A fantasy sound chip based off the 2A03, but with some improvements.

## Pulse Channels

On the 2A03's duty 3, there stands a 75 pulse that confused spectrums.
```
     ┌-┐     ┌-┐     ┌-┐     ┌-┐     ┌-┐     ┌-┐     ┌-┐     ┌-┐
     | |     | |     | |     | |     | |     | |     | |     | |
     | |     | |     | |     | |     | |     | |     | |     | |
-----┘ └-----┘ └-----┘ └-----┘ └-----┘ └-----┘ └-----┘ └-----┘ └
```
On the 8C06's, it's replaced with a 62.5 (inverted version of 37.5) pulse.
```
    ┌--┐    ┌--┐    ┌--┐    ┌--┐    ┌--┐    ┌--┐    ┌--┐    ┌--┐
    |  |    |  |    |  |    |  |    |  |    |  |    |  |    |  |
    |  |    |  |    |  |    |  |    |  |    |  |    |  |    |  |
----┘  └----┘  └----┘  └----┘  └----┘  └----┘  └----┘  └----┘  └
```     
## Bass Channel
On the 2A03's bass channel, you can't use more than a triangle wave.
```
   /\      /\      /\      /\      /\      /\      /\      /\   
  /  \    /  \    /  \    /  \    /  \    /  \    /  \    /  \  
 /    \  /    \  /    \  /    \  /    \  /    \  /    \  /    \ 
/      \/      \/      \/      \/      \/      \/      \/      \
```
On the 8C06's, you can have four volume cycles like the game boy and a sine wave.
```
Duty 0:

  /¯¯\    /¯¯\    /¯¯\    /¯¯\    /¯¯\    /¯¯\    /¯¯\    /¯¯\  
_/    \__/    \__/    \__/    \__/    \__/    \__/    \__/    \_

```
```
Duty 1:
   ┌┐      ┌┐      ┌┐      ┌┐      ┌┐      ┌┐      ┌┐      ┌┐   
  /  \    /  \    /  \    /  \    /  \    /  \    /  \    /  \  
 /    \  /    \  /    \  /    \  /    \  /    \  /    \  /    \ 
┘      └┘      └┘      └┘      └┘      └┘      └┘      └┘      └
```
```
Duty 2:
   /\      /\      /\      /\      /\      /\      /\      /\   
  /  \    /  \    /  \    /  \    /  \    /  \    /  \    /  \  
 /    \  /    \  /    \  /    \  /    \  /    \  /    \  /    \ 
/      \/      \/      \/      \/      \/      \/      \/      \
```
```
Duty 3 :
  ┌¯¯┐    ┌¯¯┐    ┌¯¯┐    ┌¯¯┐    ┌¯¯┐    ┌¯¯┐    ┌¯¯┐    ┌¯¯┐  
  /  \    /  \    /  \    /  \    /  \    /  \    /  \    /  \  
 /    \  /    \  /    \  /    \  /    \  /    \  /    \  /    \ 
_┘    └__┘    └__┘    └__┘    └__┘    └__┘    └__┘    └__┘    └_
On duty 3, it uses a sine wave.
```
