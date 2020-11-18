1.命令格式
	1./command <argument> [argument]
		注解：
		command：命令
		<argument>：必要的参数
		[argument]：可选参数
	2.sendMessage各项颜色
		面向命令：
			"用法"：使用ChatColor.AQUA
			/：使用ChatColor.GREEN
			command：使用ChatColor.RED
			<argument>：使用ChatColor.RED
			[argument]：使用ChatColor.YELLOW
	3.命令条目：
		【help系】
		/points help -> 提示命令列表 O
		【check系】
		/points check O
			- 发送者为控制台 > 提示无法查询 
			- 发送者为玩家 > 告诉玩家剩余积分
		/points check help -> 提示check的帮助
		/points check aliases -> 提示check的别名
		/points check [player] -> 提示player的积分
		【add系】
		/points add -> 提示add的语法 O
		/points add help -> 提示add的语法
		/points add aliases -> 提示add的别名
		/points add <points>
			- 发送者为控制台 > 提示无法查询
			- 发送者为玩家
				- 发送者是OP > 为发送者增加points数量的积分并提示
				- 发送者不是OP > 提示没有权限
		/points add [player] <points>
			- 发送者为控制台 > 向player增加points数量的积分并提示
			- 发送者为玩家
				- 发送者是OP > 向player增加points数量的积分并提示
				- 发送者不是OP > 提示没有权限
		【cut系】
		/points cut -> 提示cut的语法 O
		/points cut help -> 提示cut的语法
		/points cut aliases -> 提示cut的别名
		/points cut <points>
			- 发送者为控制台 > 提示无法查询
			- 发送者为玩家
				- 发送者是OP > 为发送者增加points数量的积分并提示
				- 发送者不是OP > 提示没有权限
		/points cut [player] <points>
			- 发送者为控制台 > 提示无法查询
			- 发送者为玩家
				- 发送者是OP > 为player扣除points数量的积分并提示
				- 发送者不是OP > 提示没有权限
