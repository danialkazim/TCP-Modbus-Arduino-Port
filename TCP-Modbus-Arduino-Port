#include <SPI.h>
#include <Ethernet.h>
#include "MgsModbus.h"

MgsModbus Mb;
int inByte = 0; // incoming serial byte

// Ethernet settings (depending on MAC and Local network)
byte mac[] = {0x90, 0xA2, 0xDA, 0x0E, 0x94, 0xB5 };
IPAddress ip(192, 168, 0, 177);
IPAddress gateway(192, 168, 0, 1);
IPAddress subnet(255, 255, 255, 0);


void setup()
{
Ethernet.begin(mac,ip,gateway,subnet);
  // Fill MbData
//  Mb.SetBit(0,false);
  Mb.MbData[0] = 0;
  Mb.MbData[1] = 0;
  Mb.MbData[2] = 0;
  Mb.MbData[3] = 0;
  Mb.MbData[4] = 0;
  Mb.MbData[5] = 0;
  Mb.MbData[6] = 0;
  Mb.MbData[7] = 0;
  Mb.MbData[8] = 0;
  Mb.MbData[9] = 0;
  Mb.MbData[10] = 0;
  Mb.MbData[11] = 0;
  
  
}

void loop()
{
   Mb.MbData[0]=639; 
   

//  Mb.MbmRun();
  Mb.MbsRun();
}
