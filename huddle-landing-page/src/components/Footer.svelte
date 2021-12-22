<div id="footer">
    <ion-icon name="logo-facebook" />
    <ion-icon name="logo-twitter" />
    <ion-icon name="logo-instagram" />
</div>

<style>
    #footer {
        align-self: flex-end;
    }
    #footer > ion-icon {
        color: white;
        font-size: 20px;
        padding: 10px;
        border: 1px solid white;
        border-radius: 50%;
        cursor: pointer;
        transition: color 0.3s, border 0.3s;
    }
    #footer > ion-icon:not(:last-child) {
        margin-right: 10px;
    }
    #footer > ion-icon:hover,
    #footer > ion-icon:active {
        border: 1px solid rgb(255, 73, 188);
        color: rgb(255, 73, 188);
    }
</style>
