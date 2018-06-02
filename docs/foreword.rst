※超訳です。
序文
========

Flaskを始める前にこれを読んでください。ここで、プロジェクトの目的とゴールに関するいくつかの質問に対して、また、いつFlaskを使うべきか、使わないべきかという質問にうまくいけば答えられる。

"micro"とはどういう意味か？
-----------------------

“Micro” とはWebアプリケーション全体が一つのPythonファイルに収まる、という意味ではない（実際にはそのようなこともできるが）。また、Flaskが機能性に欠けているという意味でもない。Microframeworkの"micro"は、Flaskがコアをシンプルに、かつ拡張性がありつづけることを目標にしている、という意味である。
Flaskはあなたに対して、なんのデータベースを使うか、などいろいろ決めさせるようなことはしない。
そういった決定というのは、利用するテンプレートエンジンをどれにするといったようなもので、これは簡単に変えられる。その他なんでもあなた次第で、Flaskはあなたが必要とするなんにでもなれるし、あなたが必要としないものにはならない。

デフォルトでは、Flaskはデータベース抽象化レイヤー、フォームを含んでおらず、Flaskはすでにある別のライブラリが扱えるバリデーションやその他のものについて決めていない。

そのかわりFlaskは、Flask自身に組み込んであるかのようにそのような機能を付け加えるエクステンションをサポートしている。

データベース統合、フォームのバリデーション、アップロードの取扱い、様々なオープン認証技術などを多数のエクステンションが提供している。Flaskは"micro"かもしれないが、様々なニーズに対して商用利用ができるようになっている。

Configuration and Conventions
-----------------------------

Flask has many configuration values, with sensible defaults, and a few
conventions when getting started.  By convention, templates and static files are
stored in subdirectories within the application's Python source tree, with the
names :file:`templates` and :file:`static` respectively. While this can be changed, you
usually don't have to, especially when getting started.

Growing with Flask
------------------

Once you have Flask up and running, you'll find a variety of extensions
available in the community to integrate your project for production. The Flask
core team reviews extensions and ensures approved extensions do not break with
future releases.

As your codebase grows, you are free to make the design decisions appropriate
for your project.  Flask will continue to provide a very simple glue layer to
the best that Python has to offer.  You can implement advanced patterns in
SQLAlchemy or another database tool, introduce non-relational data persistence
as appropriate, and take advantage of framework-agnostic tools built for WSGI,
the Python web interface.

Flask includes many hooks to customize its behavior. Should you need more
customization, the Flask class is built for subclassing. If you are interested
in that, check out the :ref:`becomingbig` chapter.  If you are curious about
the Flask design principles, head over to the section about :ref:`design`.

Continue to :ref:`installation`, the :ref:`quickstart`, or the
:ref:`advanced_foreword`.
