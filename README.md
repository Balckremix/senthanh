<h1 align="center"> Hi <img src="https://img.icons8.com/plasticine/100/000000/facebook.png" width="25">, I'm Sen Thanh </h1>
<h3 align="center"> Developer from Vietnames</h3>
<p align="left"> <img src="https://komarev.com/ghpvc/?username=manhkhac&color=ff69b4" alt="senthanh" /> </p>
<p align="left"> <a href="https://github.com/ryo-ma/github-profile-trophy">
  <img width=800 src="https://github-profile-trophy.vercel.app/?username=manhkhac&column=8&theme=gruvbox&no-frame=true"/></a> 
</p>
<br>
# 🤝🏻 Connect with Me
<p align="center">
&nbsp; <a href="https://twitter.com/nguyenmanh" target="_blank" rel="noopener noreferrer"><img src="https://img.icons8.com/plasticine/100/000000/twitter.png" width="100" /></a>  
&nbsp; <a href="https://www.instagram.com/manhklove1" target="_blank" rel="noopener noreferrer"><img src="https://img.icons8.com/plasticine/100/000000/instagram-new.png" width="100" /></a>  
&nbsp; <a href="https://github.com/manhkhac" target="_blank" rel="noopener noreferrer"><img src="https://img.icons8.com/plasticine/100/000000/github.png" width="100" /></a>
&nbsp; <a href="https://www.facebook.com/manhict" target="_blank" rel="noopener noreferrer"><img src="https://img.icons8.com/plasticine/100/000000/facebook.png"  width="100" /></a>
&nbsp; <a href="https://t.me/manhkhac" target="_blank" rel="noopener noreferrer"><img src="https://img.icons8.com/plasticine/100/000000/telegram-app.png"  width="97" /></a>
&nbsp; <a href="mailto:nguyenmanhict@gmail.com" target="_blank" rel="noopener noreferrer"><img src="https://img.icons8.com/plasticine/100/000000/gmail.png"  width="100" /></a>
</p>

![](https://github.com/Platane/snk/raw/output/github-contribution-grid-snake.svg)

Pull a github user's contribution graph.
Make it a snake Game, generate a snake path where the cells get eaten in an orderly fashion.

Generate a [gif](https://github.com/Platane/snk/raw/output/github-contribution-grid-snake.gif) or [svg](https://github.com/Platane/snk/raw/output/github-contribution-grid-snake.svg) image.

Available as github action. Automatically generate a new image at the end of the day. Which makes for great [github profile readme](https://docs.github.com/en/free-pro-team@latest/github/setting-up-and-managing-your-github-profile/managing-your-profile-readme)

## Usage

**github action**

```yaml
- uses: Platane/snk@v1
  with:
    # github user name to read the contribution graph from (**required**)
    # using action context var `github.repository_owner` or specified user
    github_user_name: ${{ github.repository_owner }}

    # path of the generated gif file
    # If left empty, the gif file will not be generated
    gif_out_path: dist/github-snake.gif

    # path of the generated svg file
    # If left empty, the svg file will not be generated
    svg_out_path: dist/github-snake.svg
```

[example with cron job](https://github.com/Platane/Platane/blob/master/.github/workflows/main.yml#L24-L29)

If you are only interested in generating a svg, you can use this other faster action: `uses: Platane/snk/svg-only@v1`

**interactive demo**

<a href="https://platane.github.io/snk">
  <img height="300px" src="https://user-images.githubusercontent.com/1659820/121798244-7c86d700-cc25-11eb-8c1c-b8e65556ac0d.gif" ></img>
</a>

[platane.github.io/snk](https://platane.github.io/snk)

**local**

```
npm install

npm run dev:demo
```

## Implementation

[solver algorithm](./packages/solver/README.md)
