:root {
  --blue-active: #2196f3;
  
  --black-text: #212121;
  
  --black-light: #757575;
  
  --background: #2f303a;
  
  --white: #ffffff;
  
  --bac-gray: #e5e5e5;
  
  --bac-dark-grey: #f5f4fa;
  
  --white-text-op60: rgba(255, 255, 255, 0.6);
  
  --black: #000000;
  --snw: #AFB1B8;

  --border-col: #EEEEEE;


  --dist-cards: 30px; 
}


*{
  margin: 0;
  padding: 0;
}


body { 
  font-family: "Roboto", sans-serif;
}
  
a {
  text-decoration: none;
}


img {
  display: block;
  width: 100%;
  height: auto;
}

button {
  border: 0px;
}

.list {
  padding: 0%;
  margin: 0%;
  list-style: none;
}


.container {
  max-width: 1200px;
  margin: auto;
  padding-left: 15px ;
  padding-right: 15px;
}

/* ШАПКА*/

.header {
  background-color: var(--white);
}

.page-header {
  display: flex;
  align-items: center;

  width: 1200px;
  padding: 0 15px;
 
  background-color: var(--white);
} 

.header--line {
  border-bottom: 1px solid #ECECEC;
}

.main-nav {
  display: flex;
  align-items: center;
}

.logotype {
  display: block;
  font-family: "Raleway", sans-serif;
  font-weight: 700;
  font-size: 26px;
  line-height: 1.19;
  font-style: normal;

  color: var(--black);
}

.logotype--inverse {
  color: var(--white)
}
   
.logotype__accent {
  color: var(--blue-active);
}

.container-footer__logotype {
  margin-bottom: 20px;
}

.set-pages{
  display: flex;
  margin-left: 93px;

  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 1.14;
}

.set-pages .set-pages__item + .set-pages__item {
  margin-left: 50px;
}

.set-pages .set-pages__links {
  display: block;
  padding-top: 32px;
  padding-bottom: 32px;
}

.set-pages__item .set-pages__links {
  display: flex;
  align-items: center;
}

  
.set-pages .set-pages__links .current {
  color: var(--blue-active);
}
  
.set-pages .set-pages__links {
  color: var(--black-text);
}
  
.set-pages .set-pages__links:hover,
.set-pages .set-pages__links:focus {
  color: var(--blue-active);
}
  
.set-pages .set-pages__links {
  position: relative; 
  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
  
.set-pages .set-pages__links::after {
  content: "";
  display: inline-block;
  width: 100%;
  height: 4px;
  background-color: var(--blue-active);
  border-radius: 2px;
}

.set-pages__links--current::after {
  position: relative; 
  content: "";
  position: absolute;
  left: 0;
  bottom: 0;
  display: inline-block;
  width: 100%;
  height: 4px;
  background-color: var(--blue-active);
  border-radius: 2px;
}

.contact-links {
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 1.14;
  margin-left: auto;

  display: flex;
  align-items: center;
}

.contact-links__links {
  display: flex;
  align-items: center;
}

.contacts-links .contact-links__links {
  margin-right: 50px;
}

.contact-links .contact-links__links {
  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.contact-links .contact-links__item + .contact-links__item {
  margin-left: 50px;
}

.contact-links__mail-svg {
  width: 16px;
  height: 16px;
  fill: currentColor;
  margin-right: 10px;
}

.contact-links__tel-svg {
  width: 16px;
  height: 16px;
  fill: currentColor;
  margin-right: 10px;
}

.contact-links .contact-links__links {
  color: var(--black-light); 
}
  
.contact-links .contact-links__links:hover,
.contact-links .contact-links__links:focus {
  color: var(--blue-active);
}

/* HERO*/

.hero-title {
  font-style: normal;
  font-weight: 900;
  font-size: 44px;
  line-height: 1.36;
  color: var(--white);
  text-align: center;
}
 
.hero-button {
  font-family: "Roboto", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
  line-height: 1.8;
  color: var(--white);
  background-color: #2196f3;
  outline: 0px;
}
  
.hero {
  max-width: 1600px;
  text-align: center;
  margin: 0 auto;
} 

.hero-container {
  padding: 200px 15px;

  max-width: 1600px;
  margin-left: auto;
  margin-right: auto;
  background-image: linear-gradient(
  rgba(47, 48, 58, 0.4),
  rgba(47, 48, 58, 0.4)), url("/img/Img\ 17.jpg");
  
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  
}

.hero-title {
  width: 696px;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 30px;
}
  
.hero-button {
  padding: 10px 32px;
  border-radius: 4px;
}

/* модалка */


.modal {
  position: absolute;
  top: 50%;
  left: 50%;
  padding: 40px;
  max-height: 581px;
  max-width: 528px;

  border-radius: 4px;
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.12),
    0px 1px 1px rgba(0, 0, 0, 0.14),
    0px 2px 1px rgba(0, 0, 0, 0.2);
    transform: translate(-50%, -50%) scale(1);

    transition-property: transform;
    transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
  background-color: var(--white);

  padding-top: 40px;
  padding-bottom: 40px;
  padding-left: 40px;
  padding-right: 40px;
}

.modal-button {
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  width: 30px;
  height: 30px;
  background-color: var(--white);
  border: 1px solid rgba(0, 0, 0, 0.1);
  border-radius: 50%;
  top: 8px;
  right: 8px;
  outline: 0px;
  color: $black;
}

.modal-button:hover,
.modal-button:focus {
  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);

  color: $blue-active;
  outline: 0px;
}

.modal-button__close {
  width: 18px;
  height: 18px;
  top: 3px;
  left: 4px;
  fill: currentColor;

}

.modal-title {
  font-family: Roboto;
  font-style: normal;
  font-weight: 700;
  font-size: 20px;
  line-height: 1,15px;
  color: var(--black-text);
  text-align: center;
  margin-bottom: 12px;
  letter-spacing: 0.03em;
}

/* ФОРМА */

.form-field {
  display: flex;
  flex-direction: column;
  margin-bottom: 10px;
  position: relative;
}

.form-field--placecomment {
  margin-bottom: 20px;
}


.form-filed__name {
  font-family: Roboto;
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 1,16px;
  color: var(--black-light);
  margin-bottom: 4px;
  letter-spacing: 0.01em;
}

.form-field__input {
  height: 40px;
  border: 1px solid rgba(33, 33, 33, 0.2);
  border-radius: 4px;
  padding-left: 40px;
}

.form-field__input:hover, 
.form-field__input:focus {
  fill: var(--blue-active);
  border-color: var(--blue-active);
  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.form-field__input:focus,
 .form-field__input:hover+.form-field__svg {
   outline: none;
  fill: var(--blue-active);
  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.form-field__svg {
  position: absolute;
  top: 50%;

  left: 12px;
  fill: var(--black-text);
}


.form-field__name {
  font-family: Roboto;
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 1,16px;
  color: var(--black-light);
  margin-bottom: 4px;
  letter-spacing: 0.01em;
}

.form-field__textarea {
  height: 120px;
 
  border: 1px solid rgba(33, 33, 33, 0.2);
  border-radius: 4px;
  margin-bottom: 20px;
  padding: 12px 16px;

  font-family: Roboto;
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 1.16px;
  color:rgba(117, 117, 117, 0.5);
}

.form-field__textarea:hover,
.form-field__textarea:focus {
  border: 1px solid var(--blue-active);
  outline: none;
  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1); 
}

.wrapper-checkbox__label {
  font-family: Roboto;
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 1.71px;
  color: var(--black-light);
  display: flex;
  align-items: center;
  margin-bottom: 30px;
}

.wrapper-checkbox__link {
  display: block;
  color: var(--blue-active);
  text-decoration: underline;
} 

 .wrapper-checkbox__input {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  border: 0;
  padding: 0;
  white-space: nowrap;
  clip-path: inset(100%);
  clip: rect(0 0 0 0);
  overflow: hidden;
}
  
.wrapper-checkbox__icon {
  display: inline-block;
  width: 16px;
  height: 15px;
  letter-spacing: 00.03em;
  
  border: 2px solid var(--black-text);
  border-radius: 2px;

  margin-left: 14px;
  margin-right: 9px;
}

.wrapper-checkbox__input:checked + .wrapper-checkbox__icon {
  border-color: transparent;
  fill: var(--white);
  background-color: var(--blue-active);
  background-image: url(../img/icon-check.svg);
  background-size: contain;
  background-origin: border-box;

  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1); 
}

/* Кнопка модалки */

.div-button__submit {
  width: 200px;
  height: 50px;

  border-radius: 4px;
  border: 1px solid var(--blue-active);
  color: var(--white);
  background-color: var(--blue-active);
  box-shadow:0px 4px 4px rgba(0, 0, 0, 15%);

  font-weight: 700;
  font-size: 16px;
  line-height: 1.87;
  font-family: "Roboto", sans-serif;
  outline: 0px;
}

.div-button {
 display: flex;
 justify-content: center;
}

textarea {
  resize: none;
}

/*НАШІ ПЕРЕВАГИ */

.container--advantages {
  padding-top: 94px;
  padding-bottom: 94px;
}

.visually-hidden {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  border: 0;
  padding: 0;
  white-space: nowrap;
  clip-path: inset(100%);
  clip: rect(0 0 0 0);
  overflow: hidden;
}

.set-info {
  display: flex;
  width: 1200px;
  margin: 0 15px;
}

.set-info .list + .list {
  margin-left: 30px;
}

.set-info > .list {
  flex-basis: calc((100% - 90px) / 4);
}

.list__icons {
  height: 120px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: var(--bac-dark-grey);
  margin-bottom: 30px;
}

.list__svg {
  width: 70px;
  height: 70px;
  fill: currentColor;
}

.list__title {
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 1.14;
  color: var(--black-text);
  margin-bottom: 10px;
}
  
.list__text {
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 1.71;
  color: var(--black-light);
}

/* наша робота */

.container--our-work{
  padding-bottom: 94px;
}

.our-work-title {
  font-style: normal;
  font-weight: 700;
  font-size: 36px;
  line-height: 1.16;
  text-align: center;
  color: var(--black-text);

  text-align: center;
  margin-bottom: 50px;
}

.box-our-work {
  margin: 0;
  list-style: none;
  display: flex;
  margin-left: -30px;
}

.box-our-work > .box-our-work__list  {
  flex-basis: calc(100% / 3 - 30px);

  margin-left: 30px;
}

.box-our-work__list {
  margin: 0;
  position: relative;
}
  
.employee-name {
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 1.18;
  color: var(--black-text);
}
  
.employee-position {
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.18;
  color: var(--black-light);
}

.card-thumb-container {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding-top: 27px;
  padding-bottom: 27px;
  background-color:  rgba(47, 48, 58, 0.8);
  display: block;

}

.box-our-work__card-thumb {
  position: relative;
  overflow: hidden;
}

.card-thumb-container > .box-our-work__text {
  text-align: center;
}

.box-our-work__card-thumb > .card-thumb-container {
  position: absolute;
}

.box-our-work__text{
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 1.14;
  color: var(--white);
}

/* наша команда */

.our-team {
  background-color: var(--bac-dark-grey);

  padding-top: 94px;
  padding-bottom: 94px;
}

.our-team-title {
  font-style: normal;
  font-weight: 700;
  font-size: 36px;
  line-height: 1.16;
  color: var(--black-text);

  text-align: center;
  margin-bottom: 50px;
}

.card-content {
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.18;
  color: var(--black-text);
}

.card-content__position--profession {
  color: var(--black-light);
}

.list-employees {
  padding: 0;
  margin: 0%;
  list-style: none;

  display: flex;

  margin-left: -30px;
  margin-top: -0;
}

.our-employee {
  border-radius: 5px;
  box-shadow: 0px 2px 3px rgba(0, 0, 0, 0.12),
    0px 1px 1px rgba(0, 0, 0, 0.14),
    0px 2px 2px rgba(0, 0, 0, 0.2);
  
}

.list-employees__item {
  flex-basis: calc(100% / 4 - 30px);

 
}

.card-content {
  padding: 30px 59px 30px 60px;
  
}

.card-content__position {
  margin-top: 10px;
}

.social-networks__link {
  width: 44px;
  height: 44px;
  border-radius: 50%;
  color: var(--snw);
  display: flex;
  align-items: center;
  justify-content: center;
}

.social-networks__link:hover,
.social-networks__link:focus {
  background-color: var(--blue-active);
  color: var(--white);

  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.social-networks .social-networks__elements + .social-networks__elements {
  margin-left: 10px;
}

.social-networks {
  display: flex;
  align-items: center;
  margin-top: 16px;
}


.social-networks__svg {
  width: 20px;
  height: 20px;
  fill: currentColor;
}

/*ПОСТІЙНІ КЛІЄНТИ */

.container--our-customers {
  padding-top: 94px;
  padding-bottom: 94px;
}

.our-cust-title {
  font-style: normal;
  font-weight: 700;
  font-size: 36px;
  line-height: 1,16px;
  color: var(--black-text);
  text-align: center;
  margin-bottom: 50px;
}

.customer-list {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0;
  padding: 0; 
}

.customer-list .customer-list__element + .customer-list__element {
  margin-left: 30px;
}

.customer-list__link {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 170px;
  height: 90px;
  fill: var(--snw);
  border: 1px solid var(--snw);
  border-radius: 4px;
}

.customer-list__link:hover, 
.customer-list__link:focus { 
  fill: var(--blue-active);
  border: 1px solid var(--blue-active);

  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

/* footer */

.footer {
  background-color: var(--background);
}

.footer--container {
  display: flex;
  align-items: baseline;

  padding-top: 60px;
  padding-bottom: 60px;
}

.address-box__street {
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 1.71;
  color: var(--white);
  margin-bottom: 9px;
}

  
.address-box__street:hover,
.address-box__street:focus {
  color: var(--blue-active);

  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.contact-footer {
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 1.71;
  display: block;
}

.contact-footer__meil {
  margin-bottom: 9px;
}
  
.contact-footer__link {
  color: var(--white-text-op60);
}

.contact-footer__link:hover,
.contact-footer__link:focus {
  color: var(--blue-active);

  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.join-box {
  margin-left: 70px;
}

.join__title {
  font-family: "Roboto", sans-serif;
  font-weight: 700;
  font-size: 14px;
  line-height: 1.14;
  font-style: normal;
  color: var(--white);
  margin-bottom: 20px;
}


.box-form {
  margin-left: 93px;
  
}

.box-form__text {
  font-family: "Roboto", sans-serif;
  font-weight: 700;
  font-size: 14px;
  line-height: 1.17;
  font-style: normal;
  color: var(--white);
  text-transform: uppercase;
  margin-bottom: 20px;
}

.form-footer {
  display: flex;
  align-items: center;
}

.form-footer__input {
  width: 358px;
  height: 50px;
  border-radius: 4px;
  border: 1px solid rgba(255, 255, 255, 30%);
  background-color: var(--background);

  display: flex;
  align-items: center;
  padding-left: 16px;
  
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.25;
  font-style: normal;
}

.form-footer__input:focus {
  outline: none;
}

.form-footer___button {
  width: 200px;
  height: 50px;
  border-radius: 4px;
  color: var(--white);
  background-color: var(--blue-active);
  box-shadow:0px 4px 4px rgba(0, 0, 0, 15%);

  font-weight: 700;
  font-size: 16px;
  line-height: 1.87;
  font-family: "Roboto", sans-serif;

  display: flex;
  align-items: center;
  padding-left: 29px;
  margin-left: 10px;
  border: 0px;
}


.form-footer__svg {
  width: 24px;
  height: 24px;
  fill: var(--white);
  top: 13px;
  left: 28px;
  margin-left: 10px;
}

<!-- сторінка портфоліо -->


.container {
  max-width: 1200px;
  margin-left: auto;
  margin-right: auto;
  padding-left: 15px;
  padding-right: 15px;
}

.container--portfolio {
  padding-top: 94px;
  padding-bottom: 94px;
}
  
.btn-box {
  display: flex;
  justify-content: center;
  margin-bottom: 50px;
}

.btn-box__element:last-child {
  margin-right: 0px; 
}

.btn-box__element {
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 1.62;

  margin-right: 8px;
}

.btn-box__button {
  color: var(--black-text);
  font-weight: 500;
  font-size: 16px;
  line-height: 1.62;
  font-family: "Roboto", sans-serif;

  padding: 6px 22px;
 
  background-color: var(--bac-dark-grey);
  border-radius: 4px;
  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
  border: 0px;
}
  
.btn-box__button:hover,
.btn-box__button:focus {
  color: var(--white);
  background-color: var(--blue-active);
  border-radius: 4px;
 
  box-shadow: 0px 3px 1px rgba(0, 0, 0, 0.1),
    0px 1px 2px rgba(0, 0, 0, 0.8),
    0px 2px 2px rgba(0, 0, 0, 0.12);

  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

/* сітка */

.card-filters {
  padding: 0;
  margin: 0;
  list-style: none;

  display: flex;
  flex-wrap: wrap;

  margin-top: -30px;
  margin-left: -30px;
}

.card-filters__element {
  flex-basis: calc(100% / 3 - 30px);

  margin-left: 30px;
  margin-top: 30px;
}

  
.card-filters__title {
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  line-height: 2;
  color: var(--black-text);
}
  
.card-filters__text{
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.87;
  color: var(--black-light);
  margin-top: 4px;
}


.card-filters__content {
  padding: 30px 32px;
  border: 1px solid var(--border-col);
}

.card-filters__link {
  border-radius: 5px;
}

.card-filters__element:hover,
.card-filters__element:focus {
  box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.12),
    0px 4px 4px rgba(0, 0, 0, 0.6),
    1px 4px 6px rgba(0, 0, 0, 0.16);

  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.card-filters__thumb {
  position: relative;
  overflow: hidden;
}
  
.card-filters__overlay{
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 100%;
 
  background-color: rgb(33, 150, 243, 0.9);
  transform: translateY(100%);
  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}

.card-filters__actionstext {
  font-style: normal;
  font-weight: 400px;
  font-size: 18px;
  line-height: 1.56;
  color: var(--white);
  letter-spacing: 0.03em;
  padding: 63px 24px;
}

.card-filters__link:hover .card-filters__overlay,
.card-filters__link:focus .card-filters__overlay {
  transform: translateY(0); 
  opacity: 1;

  transition-property: transform;
  transition: 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
