1.) Omogočili smo pin PA8.
1..)Poleg pina izpiše TIM1_CH1.
2.)Vrednost prescaler je 16MHz.
3.)Vrednost se spremeni na 10Hz.(1000:100)
4.)Ta parameter pomeni da gre vrednosta krivulja do polovice in se nato  ponovi.
 b.)if (HAL_TIM_OC_ConfigChannel(&htim1, &sConfigOC, TIM_CHANNEL_1) != HAL_OK)
5. a) dutyCycle+=10;
   b)if(dutyCycle>90) dutyCycle=10;(Če je duty cycle večji od 90 se spusti na 10)
   c)HAL_Delay(1000); (ukaz, ki  pomeni  zamik v  milisekundah(1000))
