##WowCombatLog##
***
分析WCL生成的文本日志文件，输出每位成员的嗑药情况

* 检查逻辑
> 1. 监控技能释放成功的记录（SPELL_CAST_SUCCESS）
> 2. 不监控BUFF情况

* 注意事项
> 1. 一个WCL文件作为一次出勤，每个团队成员在本次记录中，施法超过20次，记为出勤
> 2. 消耗品价格以AH为准，AH价格波动较大，所以每次需要重新抓取
> 3. 因使用施法监控，所以带BUFF进本将不会被统计
> 4. 如需要添加新的药剂监控，只需要修改变量buffsAndCasts即可
