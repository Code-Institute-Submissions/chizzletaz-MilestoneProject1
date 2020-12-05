goal: circle border around social media icons:
.list-inline-item {
    background-color: #6c757d;
    border: 1px solid black;
    border-radius: 50%;
    height: 40px;
    width: 40px;
    padding: 7px:
    text-align: center;
issue: the icons aren't centered: ![uncentered icons](assets/img/test/icon border 1.png)
trials: put text align after border-radius: ![uncentered icons](assets/img/test/icon border 2.png)
so horizontally centered.
for vertically centered: 

solution: .list-inline-item {
    background-color: #6c757d;
    border: 1px solid #fff;
    border-radius: 50%;
    text-align: center;
    height: 40px;
    width: 40px;
    padding: 7px;
}

