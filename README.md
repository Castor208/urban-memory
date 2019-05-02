# urban-memory
## section
### subsection
text

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

