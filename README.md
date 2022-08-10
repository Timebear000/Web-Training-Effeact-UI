# Web CSS Training Effect Clone Codeing

유트부 링크 : [https://www.youtube.com/watch?v=rc50owRPdUI&list=PLTqTKNbYVRmRrk22BX0uvzRaOggI6EB6M&index=2&t=21s](https://www.youtube.com/watch?v=rc50owRPdUI&list=PLTqTKNbYVRmRrk22BX0uvzRaOggI6EB6M&index=2&t=21s)

작성일 : 2022년 8월 10일

중요 코드

```css
.text-box h1 {
  font-size: 190px;
  line-height: 160px;
  margin-left: -10px;
  /* Effect */
  color: transparent;  /** 글자색 투명하게  */
  -webkit-text-stroke: 1px #fff; /** 글자 Border 1px  */
  background: url(images/back.png); /** 배경 화면  */
  -webkit-background-clip: text;  /** 투명한 글자 뒤에 배경화면 배치 */
  background-position: 0 0; /** 배경화면 배치  */
  animation: back 20s linear infinite; /** 애니메이션  20초 안에 0 에서 2000px 까지 이동 무한히 반복 */
}
@keyframes back {
  /* windth 값이 100%일 경우 2000 까지 이동 */
  100%{
    background-position: 2000px 0;
  }
}

```

결과물
![결과물](doc/result.gif)
