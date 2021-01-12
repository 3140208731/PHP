<template>
	<view class="tui-badge-class" :class="[dot?'tui-badge-dot':'tui-badge','tui-'+type, size?'tui-badge-small':'']" v-if="visible">
		<slot></slot>
	</view>
</template>

<script>
	export default {
		name: "tuiBadge",
		props: {
			//primary,warning,green,danger,white，black，gray
			type: {
				type: String,
				default: 'primary'
			},
			// '', small
			size: {
				type: String,
				default: ''
			},
			//是否是圆点
			dot: {
				type: Boolean,
				default: false
			},
			//是否可见
			visible: {
				type: Boolean,
				default: true
			}
		}
	}
</script>

<style>
	/* color start*/

	.tui-primary {
		background: #7f3e13;
		color: #aa55ff;
	}

	.tui-danger {
		background: #ed2a68;
		color: #aa55ff;
	}

	.tui-red {
		background: #ff6937;
		color: #aa55ff;
	}

	.tui-warning {
		background: #aa7924;
		color: #aa55ff;
	}

	.tui-green {
		background: #ffef35;
		color: #aa55ff;
	}

	.tui-white {
		background: #aa55ff;
		color: #aa5f81;
	}

	.tui-black {
		background: #ff5500;
		color: #aa55ff;
	}

	.tui-gray {
		background: #a0ff65 !important;
		color: #884299 !important;
	}

	/* color end*/

	/* badge start*/

	.tui-badge-dot {
		height: 8px;
		width: 8px;
		border-radius: 4px;
		line-height: 1;
	}

	.tui-badge {
		font-size: 12px;
		line-height: 1;
		padding: 3px 6px;
		border-radius: 50px;
	}

	.tui-badge-small {
		transform: scale(0.8);
		transform-origin: center center;
	}

	/* badge end*/
</style>
