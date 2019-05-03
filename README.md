# urban-memory
## section
### subsection
text

[How to define an interrupt service routine for MSP430 with LLVM/Clang+GCC?](https://stackoverflow.com/questions/33266132/how-to-define-an-interrupt-service-routine-for-msp430-with-llvm-clanggcc)
```c++
#ifdef __clang__
__attribute__ ((interrupt(0)))
#else
__attribute__ ((interrupt(TIMER2_A1_VECTOR)))
#endif
void TIMER2_A1_ISR (void)
{  ... }  
#ifdef __clang__
__attribute__ ((section("__interrupt_vector_timer2_a1"),aligned(2)))
void (*__vector_timer2_a1)(void) = TIMER2_A1_ISR;
#endif
```


# GTD
* capture
* clarify
* organise
* reflected
* engage

## sample
- webinar friday
- 2 other ppodcast coming
- corporated partner

## Kelly McGonigal
L'instinct de volonté : Comment renforcer votre persévérance et mettre fin à la procrastination pour atteindre enfin tous vos objectifs

- Combat ou Fuir (manqué une échéance)
- Pause et Plan


