<script>

</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Manrope:wght@500;700&display=swap');
  :root {
    --white: #fff;
    --verydark: #484e59;
    --desaturateddark: #6b7582;
    --grayishblue: #879aaf;
    --lightgrayish: #82baf2;
  }
  * {
    font-family: 'Manrope', sans-serif;
  }
  h3 {
    font-weight: 700;
    font-size: 1.4em;
    color: var(--desaturateddark);
  }
  h4 {
    font-weight: 700;
    font-size: 1em;
    color: var(--desaturateddark);
    margin-bottom: 3px;
  }
  p {
    font-weight: 700;
    font-size: 13px;
    color: var(--grayishblue);
  }
  main {
    background: var(--white);
    display: inline-flex;
    max-width: 50vw;
    min-height: 40vh;
    box-shadow: 0px 2px 15px 3px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
  }
  div.imgLeft {
    width: 40%;
    background-image: url('/images/drawers.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    border-radius: 10px 0 0 10px;
  }
  div.info {
    width: 60%;
    padding: 40px;
  }
  footer {
    position: absolute;
    bottom: 10px;
  }
  .mt2 {
    margin-top: 2px;
  }
  .mt20 {
    margin-top: 20px;
  }
  div.flb {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  div.icon-share {
    width: 30px;
    height: 30px;
    background-color: #edf2f7;
    border-radius: 50%;
    cursor: pointer;
  }
  .d-f {
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .icon-avatar {
    width: 30px;
    height: 30px;
    border-radius: 50%;
  }
  .icon-social {
    width: 30px;
    height: 30px;
  }
  .d-if {
    display: inline-flex;
    align-items: inherit;
  }
  .mr5 {
    margin-right: 5px;
  }
  .mr15 {
    margin-right: 15px;
  }
  .no-padding {
    margin-bottom: 0;
  }
  /* Tooltip container */
  .tooltip {
    position: relative;
  }

  /* Tooltip text */
  .tooltip .tooltiptext {
    visibility: hidden;
    min-width: 120px;
    background-color: var(--desaturateddark);
    color: #fff;
    text-align: center;
    padding: 10px 20px;
    border-radius: 6px;
    /* Position the tooltip text */
    position: absolute;
    z-index: 1;
    bottom: 185%;
    left: 50%;
    margin-left: -115px;
    /* Fade in tooltip */
    opacity: 0;
    transition: opacity 0.3s;
  }

  /* Tooltip arrow */
  .tooltip .tooltiptext::after {
    content: '';
    position: absolute;
    top: 100%;
    left: 50%;
    margin-left: -5px;
    border-width: 12px;
    border-style: solid;
    border-color: var(--desaturateddark) transparent transparent transparent;
  }

  /* Show the tooltip text when you mouse over the tooltip container */
  .tooltip:hover .tooltiptext {
    visibility: visible;
    opacity: 1;
  }
  @media only screen and (max-width: 767px) {
    main {
      display: flex;
      flex-direction: column;
      max-width: 90vw;
      min-height: 80vh;
    }
    div.imgLeft {
      min-width: 100%;
      min-height: 300px;
      background-image: url('/images/drawers.jpg');
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
      border-radius: 10px 10px 0 0;
    }
    div.info {
      width: 80%;
    }
    .tooltip .tooltiptext {
      min-width: 82vw;
      bottom: -100%;
      left: 0%;
      margin-left: -370px;
    }
    .tooltip .tooltiptext::after {
      border-color: transparent;
    }
    .d-if {
      justify-content: space-evenly;
    }
  }
</style>

<main>
  <div class="imgLeft" />
  <div class="info">
    <h3>
      Shift the overall look and feel by adding these wonderful touches to
      furniture in your home
    </h3>
    <p>
      Ever been in a room and felt like something was missing? Perhaps it felt
      slightly bare and uninviting. I’ve got some simple tips to help you make
      any room feel complete.
    </p>
    <div class="flb mt20">
      <div class="d-if">
        <img
          class="icon-avatar mr5"
          src="/images/avatar-michelle.jpg"
          alt="avatar" />
        <div>
          <h4>Michelle Appleton</h4>
          <p class="mt2 no-padding">28 Jun 2020 Share</p>
        </div>
      </div>
      <div class="icon-share d-f tooltip">
        <img class="tooltip" src="/images/icon-share.svg" alt="share-icon" />
        <span class="tooltiptext d-if">
          <p class="mr15">SHARE</p>
          <img
            class="icon-social mr15"
            src="/images/icon-facebook.svg"
            alt="icon-facebook" />
          <img
            class="icon-social mr15"
            src="/images/icon-twitter.svg"
            alt="icon-twitter" />
          <img
            class="icon-social"
            src="/images/icon-pinterest.svg"
            alt="icon-pinterest" />
        </span>
      </div>
    </div>
  </div>

</main>
<footer class="attribution">
  Challenge by
  <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">
    Frontend Mentor
  </a>
  . Coded by
  <a href="https://josegarciamanez.github.io/" target="_blank">
    @josegarciamanez
  </a>
  .
</footer>
