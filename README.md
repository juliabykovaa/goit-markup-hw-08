# goit-markup-hw-07
 
 @media screen and (min-width: 480px) {
            
        }
    
        @media screen and (min-width: 768px) {
            
        }
    
        @media screen and (min-width: 1600px) {
           
        }


       .header {
    border-bottom: 1px solid #ECECEC;
    
}

.nav {
    display: flex;
    align-items: center;
    @media screen and (min-width: 480px) {
        justify-content: space-between;
        margin: 10px 15px;
        position: relative;
    }
    
    @media screen and (min-width: 768px) {
        display: none;
    }
    
    @media screen and (min-width: 1200px) {
        justify-content: start;
    }

}

.nav-menu {
    display: flex;
    margin-left: 93px;
    padding-top: 32px;
    padding-bottom: 32px;
}

.nav-menu__item:not(:first-child) {
    @media screen and (min-width: 480px) {
        margin-left: 50px;
    }
    
}

.nav-menu__link {
    color: $primary-text-color;
    font-weight: 500;
    
    line-height: 1.18;
    letter-spacing: 0.02em;
    @media screen and (min-width: 480px) {
        font-size: 40px;
    }
    @media screen and (min-width: 768px) {}
    
    @media screen and (min-width: 1600px) {
        font-size: 14px;
        line-height: 1.14;
        position: relative;
    }
}

.nav-menu__link:hover,
.nav-menu__link:focus,
.nav-menu__link--current {
        color: $accent-color;
}
.nav-menu__link--current::after {
    @media screen and (min-width: 1200px) {
    content: "";
    position: absolute;
    left: 0;
    bottom: -33px;
    display: block;
    width: 100%;
    height: 4px;
    background-color: currentColor;
    border-radius: 2px;
}
    
}

.nav-menu__item:last-child {
    @media screen and (min-width: 480px) { 
        margin-bottom: 306px;
    }
   
}

.nav-menu__item:not(:last-child) {
    @media screen and (min-width: 480px) { 
        margin-bottom: 32px;
    }
   
}

.contact-menu {
    @media screen and (min-width: 1600px) {
        @include centeredFlex;
        margin-left: auto;
        gap: 30px;
    }

}


.contact-menu__link {
    color: $secondary-text-color;
    
    
    line-height: 1.14;
    letter-spacing: 0.02em;
    gap: 10px;
    transition: color $main-transition;
    &:hover,
    &:focus {
        color: $accent-color;
        svg {
            fill: currentColor;
        }
    }
    & + & {
        margin-left: 40px;
    }
    @media screen and (min-width: 480px) {
        font-weight: 500;
        font-size: 34px;
    }
    
    @media screen and (min-width: 768px) {}
    
    @media screen and (min-width: 1600px) {
        @include centeredFlex;
        font-size: 14px;
    }
}

.contact-menu__item .phone {
    @media screen and (min-width: 480px) {
        margin-top: 32px;
        margin-bottom: 64px;
        font-size: 24px;
}
}

.contact-menu__icon {
    fill: $secondary-text-color;
    align-items: center;
    justify-content: center;
    transition: fill $main-transition;
}

.menu__icon {
    @media screen and (max-width: 480px) {
    display: flex;
    justify-content: end;
}

}

.position-nav {
    @media screen and (max-width: 480px) {
        padding-left: 40px;
        padding-top: 48px;
        position: absolute;
        top: 0;
        left: -15px;
        right: 100%;
        width: 100vw;
        height: 100vh;
        background-color: #fff;
    }
    @media screen and (max-width: 1200px) {
        display: none;

    }
}

.close__icon {
    position: absolute;
    right: 0;
    top: 10px;
    &:hover,
    &:focus {
        color: $accent-color;
    }
}

.social-menu {
    @media screen and (min-width: 480px) {
        @include centeredFlex;
    }
    
    @media screen and (min-width: 768px) {}
    
    @media screen and (min-width: 1600px) {
        display: none;
    }
    
}

.social-menu__link {
    @media screen and (min-width: 480px) {
    text-decoration: none;
    color: $accent-color;
    font-weight: 500;
    font-size: 18px;
    line-height: 1.22;
    letter-spacing: 0.02em;
    }
}

.social-menu__item:not(:last-child) {
    margin-right: 20px;
    position: relative;
}

.social-menu__item:not(:last-child)::after {
    content: "|";
    position: absolute;
    right: -10px;
    top: 0;
    color: rgba(33, 33, 33, 0.2);
}

.social-menu {
    margin-bottom: 48px;
}