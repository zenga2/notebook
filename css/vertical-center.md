1.文字和图片(背景图)的垂直居中对齐

    图片:<inline-block> + <vertical-align: top>+ <height>
    文字:<vertical-align: top> + <font-size> + <line-height>(等于<height>)
    
2.文字和图片(fontIcon)

    .icon
        vertical-align: top
        &:before(或者after)
            font-size: 24px
            line-height: 40px
    .text
        vertical-align: top
        line-height: 40px
        font-size: 20px
    重点在于vertical-align: top 以及相同的 line-height，同时fontIcon设置的是:before(或者after)