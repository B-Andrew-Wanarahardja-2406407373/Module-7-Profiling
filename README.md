# Module-7-Profiling
adpro stuff

## GUI and CLI log screenshots
> i kept them in src/main/resources/image

## Improvements after optimization
> i saw quite a large change. for example, in the findStudentWithHighestGpa function, 
> he elapsed time was mostly in the 800 ms but after that most dropped to the double digits. Same with
> joinStudentNames. I seem to vaguely remember this problem getting mentioned in class. anyway, 
> the elapsed time reduced from some 20000 ms all the way down to around 1000

## Reflection
> 1. While performing tests with jmeter, things like latency and throughput while with
>> the Intellij profiler, you can see the total time, cpu time for each function call
> 2. it helps identify which parts need optimization. for example, in the joinStudentNames function
>> the number was highest on the loop, indicating that something in the loop needed optimization
> 3. I do think that the Intellij profiler is useful, as i mentioned in the previous question, it
>> helped me figure out which parts needed optimization
> 4. The largest challenge, i think, is time. when there is a lot of data, trying to test it takes half
>> an hour for me, and i think it takes up so much time, to the point i feel a bit averse to doing it
> 5. I can see which functions need optimization. and even which parts of the function take the most time.
> 6. First look at the time in jmeter, because that should be closer to the actual thing, then for seeing 
>> which parts need optimization, look at the profiler to identify them
> 7. See jmeter for time, and profiler for optimization. Strategies implemented can be like using 
>> String builder instead of +=, optimizing query calls, and others. Ensuring the correct result can 
>> be done with some unit testing
