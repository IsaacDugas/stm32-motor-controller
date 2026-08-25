# Motor Characterisation

## Objective

Determine the relationship between PWM duty cycle and steady-state
motor speed before implementing closed-loop speed control.

## Results

| PWM Duty Cycle | RPM |
|---:|---:|
| 30% | No rotation |
| 40% | No rotation |
| 50% | No rotation |
| 60% | No rotation |
| 65% | 13 |
| 70% | 21 |
| 75% | 32 |
| 80% | 42 |
| 85% | 50 |
| 90% | 61 |
| 95% | 72 |
| 100% | 73 |

## Observations

- Motor does not start below approximately 60-65% PWM.
- Above the starting threshold, RPM increases substantially with PWM.
- The relationship is nonlinear.
- Speed begins to saturate near maximum PWM.
- The L298N/motor/supply combination limits the maximum achievable speed.

## Encoder

Measured approximately 1940 counts per output-shaft revolution.

## Measurement

RPM was calculated from encoder count change over a measured time interval.
