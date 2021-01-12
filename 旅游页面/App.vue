<script>
	export default {
		async onLaunch() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style lang="less">
	/*每个页面公共css */
	.empty{
				width: 100%;padding-bottom: 20upx;padding-top: 40upx;display: flex;flex-direction: column;
				image{
					width: 30%;display: block;margin: 80upx auto 20upx auto;
				}
				text{
					color: #999;font-size:26upx;width: 100%;text-align: center;display: block;
				}
			}
			.cpy{
				width: 100%;color: #999999;font-size: 26upx;text-align: center;display: block;line-height: 80upx;position: absolute;bottom: 0;left: 0;
			}
			image{
				height: 0;
			}
</style>
