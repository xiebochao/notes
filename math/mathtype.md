## 数学公式相关

### [word2mathml](http://word2mathml.codeplex.com/) 
> Word to Mathml
### [mathjax](http://docs.mathjax.org/en/latest/output.html) 
> 让 mathml 在所有浏览器中正常显示
#### 示例
```html
<html>
<head>
<title>MathJax MathML Test Page</title>
<script type="text/javascript" async
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js">
</script>
</head>
<body>

<p>
When
<math xmlns="http://www.w3.org/1998/Math/MathML">
  <mi>a</mi><mo>&#x2260;</mo><mn>0</mn>
</math>,
there are two solutions to
<math xmlns="http://www.w3.org/1998/Math/MathML">
  <mi>a</mi><msup><mi>x</mi><mn>2</mn></msup>
  <mo>+</mo> <mi>b</mi><mi>x</mi>
  <mo>+</mo> <mi>c</mi> <mo>=</mo> <mn>0</mn>
</math>
and they are
<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mi>x</mi> <mo>=</mo>
  <mrow>
    <mfrac>
      <mrow>
        <mo>&#x2212;</mo>
        <mi>b</mi>
        <mo>&#x00B1;</mo>
        <msqrt>
          <msup><mi>b</mi><mn>2</mn></msup>
          <mo>&#x2212;</mo>
          <mn>4</mn><mi>a</mi><mi>c</mi>
        </msqrt>
      </mrow>
      <mrow> <mn>2</mn><mi>a</mi> </mrow>
    </mfrac>
  </mrow>
  <mtext>.</mtext>
</math>
</p>

</body>
</html>
```
### [mathml2word](https://github.com/scalad/MathML2Word) 
> Mathml to Word
