## Auto Connection Request Remover

This script automates the process of removing connection requests on LinkedIn. It is written in JavaScript and utilizes the `setInterval()` and `setTimeout()` methods to simulate user interaction with the LinkedIn website.

### How to Use

1. Go to https://www.linkedin.com/mynetwork/invite-connect/connections/ and log in to your LinkedIn account.
2. Open the browser console by pressing `Ctrl + Shift + J` on Windows or `Cmd + Option + J` on Mac.
3. Copy the following script and paste it into the console:

```
setInterval(() => {
    setTimeout(() => {
        document.getElementsByClassName("artdeco-dropdown__trigger artdeco-dropdown__trigger--placement-bottom ember-view mn-connection-card__dropdown-trigger artdeco-button--tertiary artdeco-button--muted artdeco-button--circle p1")[0].click()
    }, 150)
    setTimeout(() => {
        document.getElementsByClassName("display-flex align-items-center t-14 t-black--light t-normal")[2].click()
    }, 150)
    setTimeout(() => {
        document.getElementsByClassName("artdeco-modal__confirm-dialog-btn artdeco-button artdeco-button--2 artdeco-button--primary ember-view")[0].click()
    }, 150)
}, 500)
```

4. Press `Enter` to execute the script.

The script will start clicking on the "Accept" button for each connection request every 500 milliseconds. Each button click is preceded by a delay of 150 milliseconds, to simulate the time it takes for the user to click on the button.

### Disclaimer

This script automates a process that is normally done manually by the user. Use it at your own risk and discretion. The author of this script is not responsible for any consequences that may arise from the use of this script.
