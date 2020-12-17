# WSDM2018 音乐推荐系统

challenge：新歌、新歌手、新用户

## 任务

predict a probability for the target variable

## 数据（KKBOX数据集）

sample_submission

> id和target

train

> train.csv包含6个字段，msno（用户id），song_id（歌曲id），source_system_tab（标签名字），source_screen_name（用户界面名字），source_type（用户首先在移动应用上播放音乐的入口点。 入口点可以是专辑，在线播放列表，歌曲等），target（这是目标变量。 target = 1表示在用户的第一个可观察到的听歌事件后的一个月内重新听歌事件，否则为target = 0）

test

> 包含5个字段，以上和1）一致，除了缺少target字段。

歌曲

> song_id，song_length（歌曲时间，单位为ms），genre_ids（音乐类型），artist_name（歌手），composer（作曲），lyricist（作词），language（语言类型）

用户

> members.csv为用户信息，包含7个字段，msno（用户id），city（城市），bd（年龄），gender（性别），registered_via（登入方式），registration_init_time（初始登入时间），expiration_date（截止时间）

歌曲扩展信息

> song_extra_info.csv为歌曲扩展信息，包含3个字段，song_id（音乐id），song name（歌曲名字），isrc（歌曲标识）