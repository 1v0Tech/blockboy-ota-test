# blockboy-ota-test

Wegwerprepo voor één test: haalt een BlockBoy V2 een OTA-update op via HTTPS?

Dit is **geen** productie. De echte manifesten staan in de firmware-repo van
OviTech-BlockBoy. De binaries hier zijn een kopie van een lokale testbuild
(2.0.1) met het versieveld op 2.0.2 gezet, zodat het toestel de update als
nieuwer ziet en daadwerkelijk gaat downloaden.

Wat de test moet aantonen:

- certificaatvalidatie tegen `raw.githubusercontent.com` werkt
- de redirect van `github.com` naar `objects.githubusercontent.com` bij
  release-assets wordt gevolgd (de client volgt er maximaal 5)
