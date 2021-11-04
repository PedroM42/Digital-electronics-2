| **Push button** | **PC0[A0] voltage** | **ADC value (calculated)** | **ADC value (measured)** |
   | :-: | :-: | :-: | :-: |
   | Right  | 0&nbsp;V | 0   |  0023/0  |
   | Up     | 0.495&nbsp;V | 101 | 9923/99 |
   | Down   |  3.263     |   668  | 2573/257 |
   | Left   |   3.086    |  631   | 4093/409 |
   | Select |   3.837    |   785  | 6393/639 |
 |
   | none   |   0    |   0  |  |


| **Operation** | **Register(s)** | **Bit(s)** | **Description** |
   | :-- | :-: | :-: | :-- |
   | Voltage reference    | ADMUX | REFS1:0 | 00: ..., 01: AVcc voltage reference (5V), ... |
   | Input channel        | ADMUX | MUX3:0 | 0000: ADC0, 0001: ADC1, ... |
   | ADC enable           | ADCSRA |  |  |
   | Start conversion     |  |  |  |
   | ADC interrupt enable |  |  |  |
   | ADC clock prescaler  |  | ADPS2:0 | 000: Division factor 2, 001: 2, 010: 4, ...|
   | ADC 10-bit result    |  |  |  |
