<template>
  <div>
    <UPageHero title="GEEN GEZEIK, GEEN HSS" :ui="{ description: 'space-y-6' }">
      <template #top>
        <NuxtImg src="/logo_full.png" alt="Hoogspanning Hoogverraad" width="300" height="158"
          class="mx-auto -mb-20 mt-12" />
      </template>

      <template #description>
        <p class="text-lg text-muted">
          Waar ooit koeien loom kauwden op eerlijk gras, dreigt nu een voetbalveld vol kabels, kasten en knipperende
          lampjes te verrijzen. Ze noemen het vooruitgang. Wij noemen het: <strong>een verlengsnoer naar de
            hel.</strong>
        </p>
        <p class="text-lg text-muted">
          Volgens Stedin is het allemaal “noodzakelijk”. Volgens ons is ook drie keer per dag frikandel speciaal
          “noodzakelijk” – maar daar offer je de polder niet voor op. De overheid fluistert over participatie, maar het
          enige waar wij in mogen participeren is de kleur van het hekwerk.
        </p>
        <p class="text-2xl font-bold mb-4 text-primary">Boze burgers alle landen, verenigt u!</p>
        <p class="text-lg text-highlighted">
          Vandaag Soest, morgen de wereld, overmorgen groeien we allemaal op 380 volt.
        </p>
      </template>
    </UPageHero>

    <UContainer class="py-4">
      <NuxtImg src="/naald.jpg" width="1600" alt="Hoogspanningstation bij de Naald" class="w-full" />
    </UContainer>

    <UPageSection id="features" title="DRIE REDENEN WAAROM HSS EEN SLECHT IDEE IS"
      description="Ze noemen het vooruitgang. Wij noemen het een verlengsnoer naar de hel. Drie glasheldere argumenten, gebaseerd op gezond boerenverstand en minimaal één kop koffie te veel."
      :features="[{
        icon: 'i-lucide-volume-2',
        title: 'Herrie die je ziel leegzuigt',
        description: 'Een HSS zoemt niet – het fluistert je naam om drie uur ’s nachts. Na twee weken hoor je je eigen gedachten in wisselstroom en begint de hond te blaffen in morse. Rust wordt nostalgie.'
      }, {
        icon: 'i-lucide-trees',
        title: 'Polder wordt sciencefiction',
        description: 'Vandaag een reiger, morgen een transformator zo groot als een flat. Het landschap verandert van horizon in stekkerdoos. Straks moeten koeien laden via USB-C.'
      }, {
        icon: 'i-lucide-trending-down',
        title: 'Het glijdende helling-argument',
        description: 'Eerst een HSS, dan een datacenter, daarna een ruimtehaven voor Baarnse miljonairs. Voor je het weet moet je een helm op om de kliko buiten te zetten. Zo begint het altijd.'
      }]" />

    <UPageSection class="-mt-12">
      <UPageCard variant="subtle" :ui="{ container: 'p-8 sm:p-8 md:p-12' }">
        <div class="text-center space-y-6">
          <h2 class="uppercase text-2xl md:text-4xl font-bold">De <span class="text-primary">medische effecten</span>:
            wij
            hebben zélf onderzoek gedaan</h2>
          <p class="text-lg text-highlighted mb-12">
            Uit een recent, zeer specifiek en toevallig door ons geïnterpreteerd onderzoek van het RIVM blijkt dat
            langdurige blootstelling aan een HSS kan leiden tot:
          </p>
          <ul class="text-xl flex justify-center flex-wrap gap-x-3 gap-y-2 max-w-xl text-center mx-auto">
            <li>
              groene sprieten die spontaan uit je oren groeien;
            </li>
            <li>
              het oncontroleerbaar neuriën van het Stedin-wachtmuziekje;
            </li>
            <li>
              een lichte magnetische aantrekkingskracht tot frituurpannen;
            </li>
            <li>
              geheugenverlies, vooral rondom verkiezingsbeloftes.
            </li>
          </ul>
          <p class="text-lg text-muted">
            Artsen waarschuwen dat kinderen die binnen 3 kilometer van een HSS wonen later moeite krijgen met
            staartdelingen
            én met vertrouwen in de overheid. Toeval? Dachten wij ook niet.
          </p>
        </div>
      </UPageCard>
    </UPageSection>

    <UContainer>
      <UPageCard variant="soft">
        <div class="h-80 w-full max-w-xl mx-auto grid place-items-center text-center text-muted">
          (Hier plaatsen wij binnenkort het historische beeld van dappere Soesters met spandoeken, thermoskannen en
          opvouwbare stoeltjes. De revolutie, maar dan met versnaperingen.)
        </div>
      </UPageCard>
    </UContainer>

    <UPageSection title="OPROEP AAN HET LOKALE BESTUUR"
      description="Geacht college, beste wethouder, hallo mensen achter de tekentafel. Stop deze waanzin. Zet dat HSS waar het niemand stoort:
op zee, in de Eem, in Baarn, desnoods op wielen zodat het steeds ergens anders kan staan behalve hier. Luister één keer niet naar spreadsheets maar naar de menselijke maat (1,72 m, maat 43, rookt niet). De polder is geen verlengsnoer van Den Haag. Soest is geen stopcontact." />
    <UContainer>
      <UPageGrid>
        <UPageCard title="Verplaats het probleem naar iemand anders"
          description="Zet dat HSS op zee, in Baarn, of desnoods op wielen zodat het elke week ergens anders kan staan behalve hier. Mobiliteit is óók een vorm van innovatie."
          icon="i-lucide-map-pin-off" />

        <UPageCard title="Recht op analoge stilte"
          description="Elke Soester krijgt wettelijk recht op minstens 12 uur per dag zonder gezoem, geknetter of ambtelijk powerpointgeluid. Stilte is ook infrastructuur."
          icon="i-lucide-ear-off" />

        <UPageCard title="Compensatie in frikandellen"
          description="Voor elke kubieke meter beton één frikandel speciaal per huishouden. Met uitjes. Want als we dan toch genaaid worden, dan graag met saus."
          icon="i-lucide-utensils-crossed" />
      </UPageGrid>
    </UContainer>


    <UPageSection>
      <UPageCTA title="Ben je van de fake news media?"
        description="Onze woordvoerder staat jullie graag te woord met woorden, meningen en minimaal drie feiten die achteraf symbolisch bedoeld blijken. Microfoons graag op trilstand, kritische vragen op vliegtuigmodus."
        variant="subtle" :links="[{
          label: 'Stuur ons een suggestieve vraag',
          to: 'noreply@hoogspanninghoogverraad.nl',
          target: '_blank',
          trailingIcon: 'i-lucide-mail',
          color: 'neutral'
        }]" />
    </UPageSection>

    <UContainer class="py-12">
      <p class="text-center text-muted w-full max-w-2xl mx-auto">
        (Hier plaatsen wij binnenkort een QR-code voor donaties, zodat iedereen die dit leest kan bijdragen aan de
        strijd tegen onrecht. De revolutie, maar dan met een digitale collectebus.)
      </p>
      <NuxtImg src="/logo_full.png" alt="Hoogspanning Hoogverraad" width="300" height="158" class="mx-auto my-12" />
    </UContainer>

  </div>
</template>
