//Pointers and some Offsets

#define pat_GLItemMan_Instance FindPattern(EntryPoint, 0xFFFFFF,(PBYTE)"\xFF\x92\x00\x00\x00\x00\x8B\x8C\x24\x00\x00\x00\x00\x5F\x5E\xB8\x00\x00\x00\x00\x64\x89\x0D\x00\x00\x00\x00\x5B\x8B\xE5\x5D\xC2\x0C\x00", "xx????xxx????xxx????xxx????xxxxxxx") + 0x2A
#define pat_GLItemMan_GetItem FindPattern(EntryPoint, 0xFFFFFF,(PBYTE)"\x8B\x91\x00\x00\x00\x00\x85\xD2\x75\x05\x33\xC0", "xx????xxxxxx")
#define pat_GLInventory_FindPosItem FindPattern(EntryPoint, 0xFFFFFF,(PBYTE)"\x83\xEC\x0C\x53\x66\x8B\x5C\x24\x00\x66\x3B\x19", "xxxxxxxx?xxx")
#define pat_GLCharacter_ReqInvenDrug FindPattern(EntryPoint, 0xFFFFFF,(PBYTE)"\x83\xEC\x10\x53\x8B\xD9\xE8\x00\x00\x00\x00", "xxxxxxx????")
#define pat_GLGaeaClient_GetInstance FindPattern(EntryPoint, 0xFFFFFF,(PBYTE)"\xE8\x00\x00\x00\x00\x8B\x4C\x24\x10\x5F\x8B\xC6\x5E\x5B\x64\x89\x0D\x00\x00\x00\x00\x83\xC4\x10\xC2\x04\x00\xCC\x64\xA1\x00\x00\x00\x00", "x????xxxxxxxxxxxx????xxxxxxxxx????") + 0x1C
#define pat_GLCharacter_GLInventoryInstanceOffset FindPattern(EntryPoint, 0xFFFFFF,(PBYTE)"\x8D\x8B\x00\x00\x00\x00\xE8\x00\x00\x00\x00\x8B\xE8\x85\xED\x75\x0D", "xx????x????xxxxxx")
#define pat_GLCROWLOGIC_m_pLandManClient FindPattern(EntryPoint, 0xFFFFFF,(PBYTE)"\x89\x86\x00\x00\x00\x00\x89\x8E\x00\x00\x00\x00\x8B\x17\x52", "xx????xx????xxx")
#define pat_GLCharacter_ReqRebirth FindPattern(EntryPoint, 0xFFFFFF,(PBYTE)"\x8B\x86\x00\x00\x00\x00\x8D\x8E\x00\x00\x00\x00\x6A\x0A\xFF\x50\x24\x85\xC0\x0F\x84\x00\x00\x00\x00", "xx????xx????xxxxxxxxx????") - 0x1E
#define pat_GLCharacter_SkillReaction FindPattern(EntryPoint, 0xFFFFFF,(PBYTE)"\x6A\xFF\x64\xA1\x00\x00\x00\x00\x68\x00\x00\x00\x00\x50\x64\x89\x25\x00\x00\x00\x00\x81\xEC\x00\x00\x00\x00\x53\x55\x8B\xE9\x8A\x85\x00\x00\x00\x00\x84\xC0\x56\x57\x0F\x85\x00\x00\x00\x00\x8A\x85\x00\x00\x00\x00", "xxxx????x????xxxx????xx????xxxxxx????xxxxxx????xx????")

//Crow struct
m_pLandManClient \x89\x86\x00\x00\x00\x00\x89\x8E\x00\x00\x00\x00\x8B\x17\x52 xx????xx????xxx
m_pd3dDevice \x89\x8E\x00\x00\x00\x00\x8B\x17\x52 xx????xxx
m_pCrowData \x89\x46\x08\x75\x27 xxxxx
m_vPos \x8D\x8E\x00\x00\x00\x00\x8D\x57\x10 xx????xxx
m_vDir \x8D\x86\x00\x00\x00\x00\x89\x18 xx????xx
m_pSkinChar \x89\x86\x00\x00\x00\x00\xE8\x00\x00\x00\x00\x8B\x86\x00\x00\x00\x00\x8D\x90\x00\x00\x00\x00\x8B\x2A xx????x????xx????xx????xx
m_vMaxOrg \x8D\x8E\x00\x00\x00\x00\x89\x29 xx????xx
m_vMinOrg \x8D\x96\x00\x00\x00\x00\x89\x2A xx????xx
m_fHeight \xD9\x9E\x00\x00\x00\x00\x8B\x57\x0C xx????xxx
m_dwGlobID \x89\x96\x00\x00\x00\x00\x8B\x4F\x08 xx????xxx
m_dwCeID \x89\x8E\x00\x00\x00\x00\x8B\x57\x48 xx????xxx
m_dwNowHP \x89\x96\x00\x00\x00\x00\x0F\xB7\x4F\x4C xx????xxxx
m_wNowMP \x89\x8E\x00\x00\x00\x00\x8B\x57\x58 xx????xxx
m_Action \x8B\x8E\x00\x00\x00\x00\x83\xE9\x09\x0F\x84\x00\x00\x00\x00 xx????xxxxx????
m_PathActive \x8A\x86\x00\x00\x00\x00\x83\xC4\x10\x84\xC0\x0F\x84\x00\x00\x00\x00 xx????xxxxxxx????
m_dwActState \x8B\x86\x00\x00\x00\x00\x74\x05 xx????xx
m_NextPosition \x8D\x96\x00\x00\x00\x00\x8B\x02\x8B\x4A\x04\x8B\x52\x08\x89\x44\x24\x14 xx????xxxxxxxxxxxx
m_matTrans \x8D\x8E\x00\x00\x00\x00\x51\x8B\x8E\x00\x00\x00\x00\x8D\x96\x00\x00\x00\x00\x52\x8D\x46\x18 xx????xxx????xx????xxxx

//GLCharacter struct
m_sSKILLFACT \x8D\x86\x00\x00\x00\x00\x50\x51\x8D\x54\x24\x28 xx????xxxxxx
m_sPETSKILLFACT \x89\x88\x00\x00\x00\x00\x8B\x96\x00\x00\x00\x00\x8B\x47\x0C xx????xx????xxx
m_sLandEffect \x8D\x9E\x00\x00\x00\x00\x55\xEB\x03 xx????xxx
m_sActiveSkill \x8D\xBD\x00\x00\x00\x00\x57\x8D\x4C\x24\x24 xx????xxxxx
m_sRunSkill \x8B\x85\x00\x00\x00\x00\x8D\xBD\x00\x00\x00\x00\x57 xx????xx????x
m_vDir \x8D\xBE\x00\x00\x00\x00\x57\x89\x54\x24\x24 xx????xxxxx
m_matTrans \x8D\x8E\x00\x00\x00\x00\x51\x8B\x8E\x00\x00\x00\x00\x8D\x96\x00\x00\x00\x00\x52\x89\x44\x24\x30 xx????xxx????xx????xxxxx
m_sSTATEBLOWS \x8D\x96\x00\x00\x00\x00\x52\x89\x44\x24\x30\x8D\x86\x00\x00\x00\x00\x50 xx????xxxxxxx????x
m_pSkinChar \x8B\x8E\x00\x00\x00\x00\x8D\x96\x00\x00\x00\x00\x52\x89\x44\x24\x30 xx????xx????xxxxx
m_vPos \x8D\x86\x00\x00\x00\x00\x8B\x08\x89\x54\x24\x18 xx????xxxxxx
m_Action \x8B\x86\x00\x00\x00\x00\x83\xC0\xFE\xB9\x00\x00\x00\x00 xx????xxxx????
m_wTARNUM \x66\xC7\x86\x00\x00\x00\x00\x00\x00\xEB\x34 xxx??????xx
m_bCanActionMove \x8B\x85\x00\x00\x00\x00\x33\xF6\x3B\xC6\x57 xx????xxxxx
(market)m_bOPEN \x8A\x85\x00\x00\x00\x00\x84\xC0\x75\x74 xx????xxxx
m_dwActState \x81\xA5\x00\x00\x00\x00\x00\x00\x00\x00\xEB\x07\x8B\xCD\xE8\x00\x00\x00\x00\x8A\x85\x00\x00\x00\x00\x84\xC0\xC7\x85\x00\x00\x00\x00\x00\x00\x00\x00 xx????????xxxxx????xx????xxxx????????
m_bSTATE_STUN \x8A\x85\x00\x00\x00\x00\x84\xC0\x75\x61 xx????xxxx
m_sTargetID (-4 from offset) \x66\x89\xB5\x00\x00\x00\x00\xEB\x13\x81\xA5\x00\x00\x00\x00\x00\x00\x00\x00\xEB\x07\x8B\xCD\xE8\x00\x00\x00\x00\x8A\x85\x00\x00\x00\x00\x84\xC0\xC7\x85\x00\x00\x00\x00\x00\x00\x00\x00 xxx????xxxx????????xxxxx????xx????xxxx????????
m_fLastMsgMoveSend \x89\x85\x00\x00\x00\x00\xE8\x00\x00\x00\x00\x8B\xC8\xE8\x00\x00\x00\x00\x5F xx????x????xxx????x
m_sLastMsgMoveSend \x8D\xBD\x00\x00\x00\x00\xB9\x00\x00\x00\x00\x8D\x74\x24\x2C xx????x????xxxx
m_actorMove.PathIsActive() \x8A\x85\x00\x00\x00\x00\x84\xC0\x74\x2F\x8B\x84\x24\x00\x00\x00\x00 xx????xxxxxxx????
m_vTARPOS \x8D\x95\x00\x00\x00\x00\x8B\x0A\x89\x08\x8B\x4A\x04\x8B\x52\x08\x89\x48\x04\x89\x50\x08\x8B\x85\x00\x00\x00\x00\x50\x8D\xB5\x00\x00\x00\x00 xx????xxxxxxxxxxxxxxxxxx????xxx????
m_sTARIDS \x8D\x8D\x00\x00\x00\x00\x51\x83\xEC\x0C\x8B\xC4\x8D\x95\x00\x00\x00\x00\x8B\x0A\x89\x08\x8B\x4A\x04\x8B\x52\x08\x89\x48\x04\x89\x50\x08\x8B\x85\x00\x00\x00\x00\x50\x8D\xB5\x00\x00\x00\x00 xx????xxxxxxxx????xxxxxxxxxxxxxxxxxx????xxx????