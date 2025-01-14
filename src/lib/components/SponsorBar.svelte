<script>
    // Array of sponsor logos. Replace the src with your sponsor logo URLs.
    let sponsors = [
      { name: "The UPS Store", src: "/images/sponsorbar/ups_store.png" },
      { name: "Nava Wilson", src: "/images/sponsorbar/nava_wilson.jpg" },
      { name: "Geotab", src: "/images/sponsorbar/geotab.jpg" },
      { name: "Molex", src: "/images/sponsorbar/molex.jpg" },
      { name: "Alex Alexander", src: "/images/sponsorbar/alex_alexander.jpg" },
      { name: "Georges Vanier Secondary School", src: "/images/sponsorbar/georges_vanier.jpg" },
      { name: "Guerilla Printing", src: "/images/sponsorbar/guerilla_printing.jpg" },
      { name: "Sable Metal Fabrication", src: "/images/sponsorbar/sable_metal.jpg" },
    ];
</script>

<style>
  .sponsor-bar {
    height: 120px;
    display: flex;
    align-items: center;
    overflow: hidden;
    white-space: nowrap;
    position: relative;
    padding: 0;
  }

  .scroll-container {
    position: absolute;
    display: flex;
    justify-content: space-evenly;
    width: 400vw;
    height: 100%;
    box-sizing: border-box;

    animation: scroll 15s linear infinite;
  }

  .logo {
    display: inline-block;
    margin: 0 20px;
    flex-shrink: 0;
  }

  .logo img {
    height: 100%; /* Adjust as needed */
    object-fit: contain;
  }

  @keyframes scroll {
    from {
      transform: translateX(0%);
    }
    to {
      transform: translateX(calc(36px - 100vw));
    }
  }
</style>

<div class="sponsor-bar bg-gvss-dyellow">
  <div class="scroll-container py-2">
    <!-- Duplicate sponsors array to create a seamless loop -->
    {#each [...sponsors, ...sponsors, ...sponsors, ...sponsors] as sponsor}
      <div class="logo" aria-label={sponsor.name}>
        <img src={sponsor.src} alt={sponsor.name} />
      </div>
    {/each}
  </div>
</div>