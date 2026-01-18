1st section: 
Created two other test benches for the gen_tick module we made. I added wire tick_100_5,and wire tick_100_50. These were already pre-defined but I went ahead and added those as my two additional testbenches. What they mean is basically each test bench should output a 50% duty cycle, which they all do. 

for tick 2Hz, we expect 20 transition counts since we want a 50% duty cycle for 1000 ticks, since the source frequency is 100Hz and it ticks 1000 times. For 5Hz we expect 50 transitions since its a faster frequency than 2Hz meaning it needs more time to transition from 0 to 1 to get the full 50% duty cycle. Same with 50Hz, super fast signal so it transitions from 0 to 1 many times during the clock cycle. 

2nd Section: 
![alt text](image.png)