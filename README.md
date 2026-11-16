# VordLink

VordLink är inte en app för sociala medier. 
VordLink är ett starkt krypterat kommunikationsverktyg för vårdpersonal som arbetar i större team.


VordLink använder ett eget specialbyggt protokollpaket kallat Bramble för att ge totalsträckskryptering (end-to-end encryption) som fungerar både online och offline. Till skillnad från många andra appar som använder Signal-protokollet är Bramble byggt specifikt för att tåla fördröjningar och fungera utan internetuppkoppling.

Kryptografiska byggstenar i VordLink

Enligt den officiella protokollspecifikationen i VordLinks kodarkiv bygger krypteringen på fyra moderna kryptografiska funktioner:
• Nyckelutbyte (ECDH). Appen använder elliptiska kurvor (Diffie-Hellman) för att två enheter säkert ska kunna komma överens om delade hemliga nycklar när de läggs till som kontakter.

• Strömchiffer och autentiserad kryptering. Meddelanden och dataströmmar krypteras symmetriskt med snabba och säkra strömchiffer kombinerat med meddelandeautentiseringskoder (MAC) för att hindra att innehållet läses eller manipuleras.

• Kryptografiska hashfunktioner. Används tillsammans med nyckelhärledningsfunktioner (KDF) för att skapa nya tillfälliga sessionsnycklar och verifiera dataintegritet.

• Digitala signaturer. Varje användare har ett nyckelpar för att signera sin kontaktinformation och sina meddelanden, vilket garanterar att avsändaren är äkta.

Extra skyddslager i VordLink

• Forward Secrecy. Bramble-protokollet roterar och förnyar krypteringsnycklar kontinuerligt över tid. Om en enhet blir komprometterad i framtiden kan en angripare inte dekryptera gamla meddelanden.

• Krypterad lokal lagring. All historik, dina meddelanden och din kontaktlista lagras krypterat direkt på din egen enhet. Datan låses upp lokalt med ditt lösenord och sparas aldrig i molnet.

• Metadata-skydd via Tor. När VordLink ansluter via internet kapslas den redan krypterade trafiken in i Tor-nätverket. Det döljer din IP-adress och hindrar utomstående från att se vem du kommunicerar med.

• Oberoende granskad. Både källkoden och kryptografin har granskats av oberoende säkerhetsexperter, bland annat av Cure53 och i en säkerhetsgranskning finansierad av Open Technology Fund.
