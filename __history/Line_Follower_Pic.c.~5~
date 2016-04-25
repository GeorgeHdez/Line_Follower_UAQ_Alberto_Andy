#include <18f4550.h>
#device adc=10
#fuses XT,NOPROTECT,NOWDT,NOLVP
#use delay(clock=4M)

#DEFINE use_portd_lcd TRUE
#define LCD_ENABLE_PIN  PIN_D0                                    ////
#define LCD_RS_PIN      PIN_D1                                    ////
#define LCD_RW_PIN      PIN_D2                                    ////
#define LCD_DATA4       PIN_D3                                    ////
#define LCD_DATA5       PIN_D4                                    ////
#define LCD_DATA6       PIN_D5                                    ////
#define LCD_DATA7       PIN_D6 
#include <lcd.c>
void main()
{
// CONFIGURACION PWM
  setup_ccp1(CCP_PWM);
   setup_ccp2(CCP_PWM);
   setup_timer_2(T2_DIV_BY_4,250,1); // PWM de 1khz
   set_pwm1_duty(1000);
   set_pwm2_duty(500);
//CONFIGURACION LCD 
   lcd_init();
   while(TRUE)
   {
      lcd_gotoxy(1,1);
      printf(lcd_putc,"hola");
   
     
   }
}
