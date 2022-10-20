Cilj naloge: S pomočjo programskega okolja STM32CubeIDE in HAL knjižnicami sprogramirajte ARM mikroprocesor tako,da bo izvedel posamične ADC pretvorbe z izbranim potenciometrom
Postopek inicializacije periferije:
- Uporabljena razvojna plošča je NUCELO-L476RG.
- Zeldena LED je priključena na PA5 pinu, Modra LED pa na PA6. Na pin PC0 je priključen potenciometer.
- Razvojna ploščica ima 3 ADC pretvorbo.
- Trikotnik predstavlja opozorilo da je nekje med pini knonflikt. Ta konflikt resimo tako da odstranimo   pine oziroma jih nastavimo na set-reset.
- ADC ima 16 vhodnih kanalov.
-  Za branje potenciometra je izbran kanal IN5. poleg pina se izpiše ADC1_IN5.pin je PA0:
|   6 bit    |    10 bit    |    12 bit    |    16 bit     |
      | :--------: | :----------: | :----------: | :-----------: |
      | od 0 do 63 | od 0 do 1023 | od 0 do 4095 | od 0 do 65535 |
CubeMx PinOut
![image](https://user-images.githubusercontent.com/97598727/196907548-5e880fd4-4455-4788-8039-9ba11af323bc.png)


Potenciometer
![image](https://user-images.githubusercontent.com/97598727/196909676-a101905b-db8d-497a-a9a1-79f10fab568f.png)


Komentar

Zdi se mi da vse deluje brez kakrsno koli problema
