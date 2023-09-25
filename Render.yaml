from pyrogram import Client,filters
from pyromod import listen
import pyrogram,pyromod,time

StrPy = Client(" ",api_id=20851712,api_hash="bf4bf4893e7839b05cb5b52ac4871e1c")

@StrPy.on_message(filters.command("start advert"))
async def me(StrPy,msg):
	mes = await msg.chat.ask("Hi bro\nSend ad to forward and join @accesless",reply_to_message_id=msg.id)
	msgs = await StrPy.send_message(msg.chat.id,f"waited")
	async for dialog in StrPy.get_dialogs():
		
			time.sleep(1)
			
			if str(dialog.chat.type) == "ChatType.SUPERGROUP":
				try:
					await StrPy.forward_messages(dialog.chat.id, msg.chat.id, mes.id)
					await msgs.edit(f"Done Send in: @{dialog.title}\n")
				except:
					time.sleep(2)
					continue
			else:
				pass 
			
	
	
print("run")
StrPy.run()
