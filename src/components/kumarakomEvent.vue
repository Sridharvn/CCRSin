<template>
  <div class="wrapper">
    <div class="innerWrapper">
      <div class="header">
        <!-- <h2>Registration Form</h2>
          <h4>Cancer Control and Research Society</h4> -->
        <h2>HIT (How I Treat) Oncology Conference 2024</h2>
        <h6>(HOTEL LAKESONG, KUMARAKOM, &nbsp; 17TH & 18TH AUGUST 2024)</h6>
      </div>

      <div v-if="false">
        NAME: DESIGNATION: AGE: SEX: INSTITUTION: WHATSAPP NUMBER: PHONE:
        E-MAIL: FOOD PREFERENCE: Veg Non-Veg
      </div>
      <div class="payment">
        <h2>Payment Details</h2>
        <div class="paymentContent">
          <div class="paymentText">
            REGISTRATION FEE: <strong>Rs 3000/</strong><br />
            PG'S: <strong>Rs 2000</strong>/<br />
            LAST DATE OF REGISTRATION: <strong>01/07/2024</strong><br />
            NO SPOT REGISTRATION<br />
            Send information to Email ID:
            <span
              ><a href="mailto:hitoncology2024@gmail.com"
                >hitoncology2024@gmail.com</a
              ></span
            >
          </div>

          <img
            src="https://imgs.search.brave.com/VMGLvpOhAdBHOUnUti2B5aDEUkJvuwDjDDYUVgrdEkk/rs:fit:500:0:0/g:ce/aHR0cHM6Ly9sYWtl/c29uZy1ob3RlbC1r/dW1hcmFrb20uYm9v/a2VkLm5ldC9kYXRh/L1Bob3Rvcy80NTB4/NDUwLzQxNzIvNDE3/MjIwLzQxNzIyMDE1/Mi9MYWtlc29uZy1S/ZXNvcnQtS3VtYXJh/a29tLUV4dGVyaW9y/LkpQRUc"
            alt=""
          />
        </div>
      </div>
      <div class="paymentDetails">
        <h2>Account Details</h2>
        <div class="accountContent">
          <div class="accountDetails">
            <br />
            ACCOUNT NAME:
            <strong>CANCER CONTROL AND RESEARCH SOCIETY KUMARANALLOOR</strong>
            <br />
            A/C NO: <strong>0930073000000064</strong> <br />
            BANK: <strong>THE SOUTH INDIAN BANK LIMITED</strong><br />
            BRANCH:<strong> KOTTAYAM MEDICAL COLLEGE, KOTTAYAM </strong><br />
            IFSC: <strong>SIBL0000930</strong> <br />
            PAN: <strong>AADAC6129Q</strong>
          </div>
          <div class="qr">
            <a href="upi://pay?pa=qr.ccrs1@sib" target="_blank">
              <img src="./../assets/kumarakomEvent/qrCode.png" alt=""
            /></a>
            <div>UPT ID: <strong>qr.ccrs1@sib</strong></div>
          </div>
        </div>
      </div>
      <div>
        <div class="place">
          <h2>Location Details</h2>
          <a href="https://maps.app.goo.gl/wdyfRM8TYXu47fvY7" target="_blank"
            >HOTEL LAKESONG, KUMARAKOM</a
          >
          17TH & 18TH AUGUST 2024
        </div>
        <div class="phoneItemsWrapper">
          <div class="phoneItems">
            <div class="phoneItem firstPhoneItem">
              <div class="phoneItemTitle">Contact</div>
              <a href="tel:+917054777762" target="_blank">+917054777762</a>
            </div>
            <div class="phoneItem">
              <div class="phoneItemTitle">Prof. Dr. C. S. Madhu MD, DNB</div>
              <a href="tel:+919387103803" target="_blank">+919387103803</a>
            </div>
            <div class="phoneItem">
              <div class="phoneItemTitle">Dr. Manoj S. MD, DM</div>
              <a href="tel:+919495685121" target="_blank">+919495685121</a>
            </div>
          </div>
        </div>
      </div>

      <div class="link">
        <div class="pdfDownload">
          <a
            href="http://www.ccrsindia.in/hit-24-registration.pdf"
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
// * {
//   outline: 1px solid red;
// }
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
  background: #fce4df;
  border-radius: 1rem;
  padding: 20px;
  margin: 10px;
  margin-block: 30px;
  width: 90vw;
  padding-inline: 30px;
  text-align: center;
}

.header {
  text-align: center;

  h2 {
    font-size: 2.5rem;
    margin-bottom: 10px;
    color: var(--text-color-dark);
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
.firstPhoneItem {
  border-right: 1.5px solid var(--text-color);
  padding-right: 20px;
}
.phoneItemsWrapper {
  display: flex;
  justify-content: center;
  width: 100%;
  .phoneItems {
    display: flex;
    justify-content: space-evenly;
    align-items: space-between;
    // flex-wrap: wrap;
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
  }
  a {
    font-size: 1.1rem;
    text-decoration: none;
  }
}
.payment {
  .paymentContent {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    img {
      width: 20vh;
    }
  }
  .paymentText {
    text-align: left;
  }
}
.paymentDetails {
  margin-top: 20px;
  .accountContent {
    display: flex;
    justify-content: space-between;
    align-items: center;
    // flex-wrap: wrap;
  }
}
.pdfDownload {
  display: flex;
  justify-content: center;
  width: 100%;
  margin-bottom: 20px;
}
@media screen and (max-width: 950px) {
  .paymentContent {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    flex-wrap: wrap;
    img {
      width: 20vh;
      display: none;
    }
    .paymentText {
      text-align: center;
    }
  }
  .firstPhoneItem {
    border: none;
    border-bottom: 1.5px solid var(--text-color);
    padding-bottom: 10px;
  }
  .phoneItemsWrapper {
    .phoneItems {
      flex-direction: column;
      .phoneItem {
        .phoneItemTitle {
          height: fit-content;
          font-size: 1.2rem;
          margin-bottom: 5px;
        }
      }
    }
    a {
    }
  }
  .paymentDetails .accountContent {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
<script>
export default {};
</script>
