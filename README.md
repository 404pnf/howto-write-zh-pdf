# -*- coding: utf-8 -*-

# install

gem install prawn

# 支持中文方法一
参考： <http://www.liangwenke.com/blog/102>

  pdf = Prawn::Document.new
  # zh-cn language
  # 需要制定字体
  pdf.font "#{Prawn::BASEDIR}/data/fonts/gkai00mp.ttf"
  pdf.text "中文"
  pdf.render_file "chinese.pdf"

# 支持中文方法二

  Prawn::Document.generate("zhognwen.pdf") do |pdf|
    pdf.font "#{Prawn::BASEDIR}/data/fonts/gkai00mp.ttf"
    pdf.text "中文字符"
  end

# 详细帮助
<https://github.com/prawnpdf/prawn>

该软件有手册，是pdf格式的。值得快速浏览一下。功能比较强大。
