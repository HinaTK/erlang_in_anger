
# Discarding Data
# 丢弃数据
When nothing can slow down outside of your Erlang system and things can’t be scaled up, you must either drop data or crash (which drops data that was in flight, for most cases, but with more violence).<br>
It’s a sad reality that nobody really wants to deal with. Programmers, software engineers, and computer scientists are trained to purge the useless data, and keep everything that’s useful. Success comes through optimization, not giving up.<br>
However, there’s a point that can be reached where the data that comes in does so at a rate faster than it goes out, even if the Erlang system on its own is able to do everything fast enough. In some cases,  It’s the component after it that blocks.<br>
If you don’t have the option of limiting how much data you receive, you then have to drop messages to avoid crashing.
<p></p> <font color="green">
&emsp;当没有什么可以减缓从外界输入到Erlang系统的数据时，并且系统也不能按比例扩大时，你就必须要丢弃一些数据，不然就会崩溃掉。(丢弃运行中的数据（data that was in flight），对于大多数的场合，可能会更加粗暴）。<br>
&emsp;这是个悲伤的事实：没有人真的想丢弃。程序员，软件工程师，或计算机科学家都被告之要减少没用的数据，并保持所有都是有用的数据，成功来自于优化，而不是放弃。<br>
&emsp;然而，必须要指出的一点是：为什么数据的输入会比输出快得多，即使在Erlang系统自身可以快速处理一切的时候，有时候，把各部分都组合在一起，就会阻塞住了。<br>
&emsp;如果你并想选择限制系统收到的数据，那么你就不得不丢弃一部分数据来防止崩溃。
</font> <p></p>
