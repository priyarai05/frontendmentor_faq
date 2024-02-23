# Responsive UI

## Apply loop over a div in JS
## Used Toggle button to hide and show the answer on questions

let questionContainer = document.querySelectorAll('.question');


questionContainer.forEach(item => {
    let answer = item.getElementsByClassName("answer")
    let img = item.querySelectorAll('img')

    img[0].addEventListener("click", () => {
        if (answer[0].classList.contains("tgl")) {
            answer[0].classList.remove("tgl")
            img[0].src = "icon-minus.svg"
        } else {
            answer[0].classList.add("tgl")
            img[0].src = "icon-plus.svg"
        }
    })
});
