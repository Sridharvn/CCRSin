<template>
  <div class="wrapper">
    <div class="innerWrapper">
      <div class="header">
        <!-- <h2>Registration Form</h2>
          <h4>Cancer Control and Research Society</h4> -->
        <h2>H I T (How I Treat) Oncology 2024</h2>
      </div>

      <div v-if="false">
        NAME: DESIGNATION: AGE: SEX: INSTITUTION: WHATSAPP NUMBER: PHONE:
        E-MAIL: FOOD PREFERENCE: Veg Non-Veg
      </div>
      <div class="payment">
        Payment Details REGISTRATION FEE: Rs 3000/- PG'S: Rs 2000/- LAST DATE OF
        REGISTRATION: 01/07/2024 NO SPOT REGISTRATION Send information to Email
        ID:
        <span
          ><a href="mailto:hitoncology2024@gmail.com"
            >hitoncology2024@gmail.com</a
          ></span
        >
      </div>
      <div class="paymentDetails">
        <div class="accountDetails">
          <h2>Account Details</h2>
          <br />
          ACCOUNT NAME: CANCER CONTROL AND RESEARCH SOCIETY KUMARANALLOOR <br />
          A/C NO: 0930073000000064 <br />
          BANK: THE SOUTH INDIAN BANK LIMITED BRANCH: KOTTAYAM MEDICAL COLLEGE,
          KOTTAYAM <br />
          IFSC: SIBL0000930 <br />
          PAN: AADAC6129Q
        </div>
        <div class="qr">
          <a href="upi://pay?pa=qr.ccrs1@sib">
            <img src="./../assets/kumarakomEvent/qrCode.png" alt=""
          /></a>
          <div>UPT ID: qr.ccrs1@sib</div>
        </div>
      </div>
      <div>
        <div class="place">
          <h2>Location Details</h2>
          <a href="https://maps.app.goo.gl/wdyfRM8TYXu47fvY7"
            >HOTEL LAKESONG KUMARAKOM</a
          >
          17TH & 18TH AUGUST 2024
        </div>
        <div class="phoneItems">
          <div class="phoneItem">
            <div class="phoneItemTitle">Contact</div>
            <a href="tel:+917054777762">+917054777762</a>
          </div>
          <div class="phoneItem">
            <div class="phoneItemTitle">Prof. Dr. C. S. Madhu MD, DNB</div>
            <a href="tel:+919387103803">+919387103803</a>
          </div>
          <div class="phoneItem">
            <div class="phoneItemTitle">Dr. Manoj S. MD, DM</div>
            <a href="tel:+919495685121">+919495685121</a>
          </div>
        </div>
      </div>

      <div class="link">
        <div class="pdfDownload">
          <a
            href="https://www.ccrsindia.in/hit-24-registration.pdf"
            target="_blank"
            >Download the Registration Form</a
          >
        </div>
      </div>
    </div>
  </div>
</template>
<!-- <style lang="scss" scoped>
.wrapper {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  color: var(--text-color) !important;
}
.innerWrapper {
  margin: 10px;
  width: 75vh;
}
.header {
  text-align: center;

  h2 {
    font-size: 2.5rem;
  }
  h4 {
    font-size: 1.5rem;
  }
  h6 {
    font-size: 1rem;
  }
}
.accountDetails {
  margin: 10px;
  h2 {
    font-size: 2rem;
    margin: 0 0 0 0;
    padding: 0 0 0 0;
  }
}
.place {
  display: flex;
  flex-direction: column;
  margin-block: 20px;
}
.qr {
  img {
    width: auto;
  }
}
</style> -->

<style lang="scss" scoped>
a {
  color: var(--text-color) !important;
  font-weight: bolder;
}
.wrapper {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  color: var(--text-color) !important;
}

.innerWrapper {
  margin: 10px;
  width: 75vh;
  text-align: center;
}

.header {
  text-align: center;

  h2 {
    font-size: 2.5rem;
    margin-bottom: 10px;
  }

  h4 {
    font-size: 1.5rem;
    margin-bottom: 10px;
  }

  h6 {
    font-size: 1rem;
    margin-bottom: 10px;
  }
}

.accountDetails {
  margin: 10px;
  text-align: left;

  h2 {
    font-size: 2rem;
    margin: 0;
    padding: 0;
  }
}

.place {
  display: flex;
  flex-direction: column;
  margin-block: 20px;
  h2 {
    font-size: 2rem;
    margin: 0;
    padding: 0;
  }
}

.qr {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 20px;

  img {
    width: 200px;
    margin-bottom: 10px;
  }
}
.phoneItems {
  display: flex;
  justify-content: space-evenly;
  align-items: space-between;
  flex-wrap: wrap;
  border: 1px solid var(--text-color);
  border-radius: 1rem;
  padding: 1rem;
  margin: 2rem;
  width: 100%;
  .phoneItem {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 10px;

    .phoneItemTitle {
      height: 30px;
      font-size: 1.2rem;
      margin-bottom: 5px;
    }
  }

  a {
    font-size: 1.1rem;
    text-decoration: none;
  }
}
.payment {
}
.paymentDetails {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
.pdfDownload {
  display: flex;
  justify-content: center;
  width: 100%;
  margin-bottom: 20px;
}
</style>
<script>
export default {};
</script>
