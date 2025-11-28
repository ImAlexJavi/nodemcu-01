# Microprocessor - Blinkande ljus
Med hjälp av microprocessorer så kan man skapa många olika små enheter. Med hjälp av programmering som C++ så kan man säga till vad microprossesorn ska göra och dens uppdrag.

Inom Arduino så finns det redan exempel kod som blink genom att gå in på `File > Examples > 01.Basics > Blink`. Detta kommer ge en exempel kod på en enkel funktion för att det ska blinka
<img width="1390" height="1275" alt="image" src="https://github.com/user-attachments/assets/320205b2-c611-4c0b-afde-3313f4101a72" />

## Förklaraing av kod
<img width="1615" height="586" alt="image" src="https://github.com/user-attachments/assets/49871805-64cf-43b2-a848-232935a976b8" />

Inom `setup` så står det `pinMode(LED_BUILTIN, OUTPUT);`. Detta säger till vilken pin den ska använda men sedan specificerar att det är inbyggda ljuset och sedan att det ska skicka ut en signal.

Nästa kod del är `loop` som är som det låter, koden som är inom loop funktionen kommer att köras om i flera varv tills man säger något annat. Inom `loop` funktionen står det `digitalWrite(LED_BUILTIN, HIGH);` detta tänder ljuset men vi vill hålla den tänd under en längre tid, annars så släks den innan vi märker av ljuset. Detta gör vi med en `delay` i detta fall är den satt på `1000` milisekunder (en sekund). Sedan är samma sak med släka `digitalWrite(LED_BUILTIN, LOW);` 

## Skicka koden så det körs
<img width="200" height="98" alt="image" src="https://github.com/user-attachments/assets/1a316233-dca6-494a-a217-61a9dc317928" />
Första steget är att varifiera koden genom att trycka på "checkmark" knappen, det kan ta ett tag tills den laddat klart. Nästa steg är att ladda upp koden in till mikroprocessorn genom att trycka på pilen. Efter det har laddat bör microprossesorns ljus blinka.
