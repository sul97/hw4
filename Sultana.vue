<template>

<div class="container">
<nav class="navbar navbar-expand-lg navbar-light bg-light " >
  <div class="container-fluid" style="background-color: #c7d9e9;">
     
         <div class="d-flex ml-auto">
                    <ul class="navbar-nav px-5 py-5 " style="background-color: #c7d9e9;">
                      <li class="nav-item">
                      <a href="#" class="nav-link">القائمة الرئيسية <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" fill="currentColor" class="bi bi-house-door" viewBox="0 0 16 16">
                        <path d="M8.354 1.146a.5.5 0 0 0-.708 0l-6 6A.5.5 0 0 0 1.5 7.5v7a.5.5 0 0 0 .5.5h4.5a.5.5 0 0 0 .5-.5v-4h2v4a.5.5 0 0 0 .5.5H14a.5.5 0 0 0 .5-.5v-7a.5.5 0 0 0-.146-.354L13 5.793V2.5a.5.5 0 0 0-.5-.5h-1a.5.5 0 0 0-.5.5v1.293L8.354 1.146ZM2.5 14V7.707l5.5-5.5 5.5 5.5V14H10v-4a.5.5 0 0 0-.5-.5h-3a.5.5 0 0 0-.5.5v4H2.5Z"/>
                      </svg></a> </li>
                       <li class="nav-item">
                        <a href="#" class="nav-link">منتجاتنا  <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" fill="currentColor" class="bi bi-moon-stars-fill" viewBox="0 0 16 16">
                            <path d="M6 .278a.768.768 0 0 1 .08.858 7.208 7.208 0 0 0-.878 3.46c0 4.021 3.278 7.277 7.318 7.277.527 0 1.04-.055 1.533-.16a.787.787 0 0 1 .81.316.733.733 0 0 1-.031.893A8.349 8.349 0 0 1 8.344 16C3.734 16 0 12.286 0 7.71 0 4.266 2.114 1.312 5.124.06A.752.752 0 0 1 6 .278z"/>
                            <path d="M10.794 3.148a.217.217 0 0 1 .412 0l.387 1.162c.173.518.579.924 1.097 1.097l1.162.387a.217.217 0 0 1 0 .412l-1.162.387a1.734 1.734 0 0 0-1.097 1.097l-.387 1.162a.217.217 0 0 1-.412 0l-.387-1.162A1.734 1.734 0 0 0 9.31 6.593l-1.162-.387a.217.217 0 0 1 0-.412l1.162-.387a1.734 1.734 0 0 0 1.097-1.097l.387-1.162zM13.863.099a.145.145 0 0 1 .274 0l.258.774c.115.346.386.617.732.732l.774.258a.145.145 0 0 1 0 .274l-.774.258a1.156 1.156 0 0 0-.732.732l-.258.774a.145.145 0 0 1-.274 0l-.258-.774a1.156 1.156 0 0 0-.732-.732l-.774-.258a.145.145 0 0 1 0-.274l.774-.258c.346-.115.617-.386.732-.732L13.863.1z"/>
                          </svg></a>
                      </li>
                      
                    </ul>
                    
                  </div>
                  
                    <div class="d-flex justify-content-between">
                        <h1  style="color: #0a0a0a; font-family:Cairo;">الوجبات السريعة</h1> 
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-fire" viewBox="0 0 16 16">
                         <path d="M8 16c3.314 0 6-2 6-5.5 0-1.5-.5-4-2.5-6 .25 1.5-1.25 2-1.25 2C11 4 9 .5 6 0c.357 2 .5 4-2 6-1.25 1-2 2.729-2 4.5C2 14 4.686 16 8 16Zm0-1c-1.657 0-3-1-3-2.75 0-.75.25-2 1.25-3C6.125 10 7 10.5 7 10.5c-.375-1.25.5-3.25 2-3.5-.179 1-.25 2 1 3 .625.5 1 1.364 1 2.25C11 14 9.657 15 8 15Z"/>
                          </svg>
                        </div>
                        &nbsp;&nbsp;&nbsp;
                    <div class="d-flex">
                        <img  alt="avatar image" class="rounded-circle"  src="https://w7.pngwing.com/pngs/193/660/png-transparent-computer-icons-woman-avatar-avatar-girl-thumbnail.png" height="35"/>
                    </div> 
                </div>
            </nav>

  <div class="container">
    <div class="row">
      <div class="col-sm-2">
        <div class="alert alert-primary"><h5 style="font-family:Cairo">المجموع : {{total}}</h5> </div>
      </div>
     <div class="col-sm-10">
      <div class="alert alert-success text-center"><h4 style="font-family:Cairo">الساندوشات </h4></div>
     </div> 
    </div>
    
    <div class="row">
     
      <div class="col " style="background-color: #faf6bc;">
      
        <div class="d-flex justify-content-between">
          <div class="p-4">
            <input type="checkbox" @change="GetTotal(Borger)"/>
          </div>
          <div class="p-4">
            <h4>{{Borger}}</h4>
          </div>
          <div class="p-4">
            <h4 style="font-family:Cairo">هامبرجر</h4>
          </div>
           <div class="d-flex">
            <img  alt="avatar image" class="rounded-circle"  src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAoHCBUUFBcVFRQYGBcZGR0dGhoaGhoZHB0dHBoZGhwZHhwaISwjGh0pIBoaJDYkKS0vMzMzGiI4PjgyPSwyMy8BCwsLDw4PHhISHjIqIykyNDMyNDIyOjIyMjIyMjIyMjQyMjI0LzIyMjIyMjI0NzI0NDIyMjIyOjIyMjIyMjIyMv/AABEIAOEA4QMBIgACEQEDEQH/xAAcAAACAgMBAQAAAAAAAAAAAAAEBQMGAAECBwj/xABHEAACAQIEBAMFBQYEAwYHAAABAhEAAwQSITEFQVFhInGBBhMykbFCocHR8CMzUmJy4RQVU4JzovEWQ5KTsuIHNIOzwtLT/8QAGgEAAgMBAQAAAAAAAAAAAAAAAgMAAQQFBv/EAC0RAAICAQQBAgUEAwEBAAAAAAABAhEDEiExQQQTUSJhcYGRMqHB8BRCsWIj/9oADAMBAAIRAxEAPwBViHkk0Exmpbz1xaFUthxy2lZhtWrnENRPDbUkVAeywYO1oBXeIMz2qfD24WaXXpzhfU0KLZDibcLW7SaCusSJaOlSD4T5VXLC6AHuSxoN9TUz2zv1qMJ4qp8lpbHF0ijrA8FA3V1oy2NIqMNIU4g+KisFZlpNSthczUW4Fte9Ry6BUTrEXwqwNzpQ+Hw/Oo8PaNxp6Ua+nhHPSpwWE8PTWaPvX5OWhLPgWanwST4jzq66JdbnTpNT4a1FYTJ8q76VogqM03ZKyTrUfuqm5RULPTELYPi2gVVcVcljTviTmKQlPFQSY2EQnDLTnhm9KrNunGAt6TQLdhvgh9oL0gKOZp17P4fKg8qq+Nl7yrV34emVBVAyCaytxWVQB5K7SakzQKgU1tjUHGKMxp9wuxSvA2ZNWjB2ojtVMpB3u8qxSO4fGWpljsXCn5Uka5y61UtkXFBGWda0rHap1Twio7dskwoLHkAJNAg2CYl9aED60yXhz3Hi5NpRoSRJ05RTOxwTCE+7U3MxB/aOxUDyCiPnQepBcsLTLpFVuHWplvgc6uKcNKsVt4e26CAzqoaV5kG5MsBOg500ucUtLAS37yI1bKMpHSBvSnngudv70GoS6VlFS1ckAWrkkSBkbUbyNNRW8TwvFSuaxc8Xw6T8429auTcWaVZQ0iQQxBUj+mBrpvPWiMOt7w3PeeFmBK6yublk3MTHbehj5UZP4U2SWOaW9IptjAXkUfsnkmB4TvWNwfFZtbLiPL86sOMutnYB2KhtIlVBjkJ0iSKnsLfuIct0mJBQkEx2J3mgXmJyaS3DeBqKbaK62GvSqm24/wBpox1a2viUrPURTW29y3ZVlcGTGQgZl1I1kSdqY3cQWQIhF47spXIYHME6bkD1psPLje6FTxPor1m3ArpH1PQVYgEdFuXAqbj3bCCCCQZMgzptShThmbKVcAmAVMgmdDDa1p/y8aq3ViPQm7pEKSR51BiDFPU4Q4J1hRsTGvy2pRxTh11S0AMBqSCD90zWhZYvsVpYh4hc0j1pYlvnU+KaT51nKBQyY2Ko3bubU6wrRbqvpvT5zkt+lRcFy5AeGJ7y+W6VeEEACqp7L2Zlupq186ECW7NzWVusqAnkCbVoHWpcsCpcFZkzUQY04Wms05N/KO9B4a1lAHWh8Xd10qJdlt9GYtyxHSorSS1aDaTTn2e4d7wm46nIPh5Bj+QpcmEtjMPh2uESCLY3I38hTm4y2xlspl01I+I+polbQAgaRyFaCZSrEaZh9dqTJyaoYtN2R4nCj3RdV+DVi052JGwHTX1rniNtQLYRSqnTMRGc6GNenXvRRYNcuPd8DKq5EMGYkgkDQyfrUeItkoLruWJaFB6dug0PoKRkjtsv6hkJO1b/AKwRfd21UMLj+ISEnKqzr3Y+X/WLiKgO3uVhY8IMiTEnfvUtx/8ApUQmRz1BjrqNPWsM5f60a4xp6rGGJw1trlpLYKFhmzNmG0Eb7nTasx2MuLdIUhSgKTG+zEgGYreIW6Ltq5c0yyVXkREREyDLAz2FCYu4blxrjDVuQ5aAD1iiyy0J6dm3+1AY46mtW6r67g7iSWJJJ1M9etEYTFNb8QBPYHeJjbzrVuyGZQTHUxOWRv8ArrUmJtBGAzBhGhEff0NZIqS+L2NDcX8LGNzCI9xNFVWBOZCSWYRpHLcnntSa4mVj8QiQOR0JiecmisE4Rw7KCB0+Id/lIjvWYhveXGcnc6achoNOsU/JkjKCktnYqEZRlT3VEi8MzqMhGYrJzKwEnoY8XzqWxcsg5Wt6RBaZIYdI5day3iHVCit4YiNDA7TtWWMCGtFwecAaySDH96ikm/8A5rerd/wC06+N7XtQVg7KuIT92VIZd3zHkAdhFAvhGUpbIt3BlOU/CSBoVzdaxsM6QxQg8txNHWMP7tWdCHBAzK3xfdz11p0ZOapqq5+gtx0bp3fH1BFw1t19xctMDyBlu8gjVTHTSlHE+C2WbLaYWXXQhpKHuDy86tNrGMzrAyrsegMGJPpFRPbuM0Ott1JI17cpjQ05ZZRitLb3rgU4pyepVt7lBHB7yv4rbFQfiUZlMcwRyrji+J8OQbmvQ7ijDrCgjxHTUqVJOk8iOlR3uE2r9shrKAMCysIzK3Jq2489vS+exE4UrXBX/Z6xltjypylDYfDtbXKw127UQhp633EskrK1WVZR5EzEnSnfC8PsIpfw61J1q14ewFWqvoMFxLwKXXFPIE+lMriyewpxwJ0CMsqTMxzFFtwC5UrKwEkRtVt4MSuHUbmdOkFufaucThkuNHu5O87AdyeQri4j20JtqzAbBCH3/pmKz5JKLabX5L9RS6DsTigjIDqXn5gj8D91auIJEkkgyOx6iOdIrWMhlF8ZY5kAEQZy5hoZOlNGxqsJB++sqzwlvew/S10TudGIGZt99SRyn8KGt32OUFWhQQJ5TrXL3+YPlQ9y6LkB2Yd1Oomqc0+BkEGO4oUYkB0AMEHMNJ1XUz+t6iXBPlgXFYAbkmT6RudKmXAW7bj9obhZJgwRErtGoE8j2pUoOT1JUPU0lQwTENiHAU5oJG8bAEjsNRUVx9Cdz08uVRW+LW0ec4UhSu2mscu0CokxNqJW4CT+p0rPkS7dvsZDbrYOZUySpf3hjlA5T91R5JovD4i2baqyDNGrKRvzMzO/UVxw2yrFveNGWNJjcTPl/eqnj1NKLXH0/JUZ6U27OFSaMN1MhBRcwGhHXr19JqCBmOX4ZMeVdxS1cU0uw3Uqs5w6CBmJHfkB1PaiL1hRlhg07R1G221QbaUXaw2oIaCNR+ue9TEm1pr7g5HTuwj3d10KSQI+18996k98FuGVg5QFHfUkz8vlXN1meAx22/PzrkWtetb3Jr9N/VmWk/1V9jtbyjXLJYQ3QxsR86gCbhScvrRKJWih8qGSk+SJpcA6JJysSQd9fkfMVHbzJKBvDP47joKOyEmAJ0n9d65S3rJExQaHtX5/gvUuzjiKwF0B/iHXTQg0sRTAPI06NmV9THbWgLmHCnXY7/nWmOaUJ2/0v9hThGUaXKBc1bqT3H8wrK2evD3EenL2KHwrDbU5uGFqLB2sq1Bir2p6CmRXbI99iOyoa5kY6EE10LC2TnUNmBkGT946ULgC7XC4ClU+IkxE9BzNGYwp7tmV2OXdYPM1x/OzTjkSi6BlzQxwXHjo72zkJhiiltuw1pr/AJdYI95aUByZBHhPkdiPI0iCG3aUKzEqJ/lljJEct6LwOMYrogcmdjqe3lXP8nLO3fLQMa6DcZhbdy3FxfETGYCdeRPaqre4RctvKyPUwRVnsOtv4RAjVQwaJ3kAn50i4txc27ptBBc0DCWynUde20eVJx5XNVFbr8NGvHP3A8RZvKM4OaOupAgbEaiq/Y4/dMhsgg6ZmifWI+ZFNOIcRv3EjKETnGpPYnpSP/ChiBlPmYH/AFrpeK5JfHRqjFPgYDj9xSJUkSB4Sr89hlJ1qaz7QiWLEglRqwg6MfCNP5t6TvgEkgfSo24aK0ynj4HRwyLLY4zbbdVYRrr6zRScTQCVQBT0G/LcVSbvD9yN+fP11+tCul1RGdsvTMY+U1Sxwl2DKLieqNdEZihXrP4xsDRmCxVx8wtgMQNZj5a89Dp2ryXDcXxNuQrsdI1JMAbR0pthvbLFowZlRjpmOUgsBtMGJ796GXjb2mVcq4PSFx4MaQeY6URbxS7VQLPtYrsS1p5YknIVbU6nSZplhfaPBEQ990ufzIco9QNPnWd+PlT4Lc4ot9u7zpjZWUFwbGD89jVNwPGbTghLgcqCTlk6DmNNaa4Ti4W2EObKx8IKtInWNtB51eNON6l1+4OR3VFiW5U2HuKykzry7edV+3xJG1Vg3X9cqMwnEUFvKSMxidvOnY8m+/sZ5x22HVpwV1EMNyNj3re9LkxEgwR86lwOKOzHnp5U6M7pMW41bGCJsa7y10IrGcCtUcewlzOYjuP1p5VwyAjUdq797pWlZSN6jguClIA/wy1ujcorKV6C9g/UfuecvdAG9JeJ8QRILHSa6xF0ganU1XOPpmSQdRWub6RWNdsJfi6DVNzy7elH8Gx17ENkBOVfiMDReX9RqqYCy9zLbS2S5MDSN+/SvScLw/8Awtu1aRoGrXXHNtBE8hJismWMJJ6kXn0xj02wrG4ZxZQBpkNOgHlI8udB+zNgi5cIZVYCNdeY0EbRpPpTTEYjPbDqwOWRp8j6gzSPC3ctwMhgydPPcRz61xvLik2oPlGSDfYVxfBsr2zbGT3jkPlPwwM2ZexgjlrHlVZ41IvGSW/mJknbnVixVwupLbBspI2B1g9pqpcTS+CSysy5jBAB05HTXai8WPwpOr/6NUtyG9xG4NFaO9RrxC4QQTmBMmQC06bMRI261BcuD7QK9dDWmuJGiOe5hfureo0qofHJ3YQuOYcpqQY/qpFCIUOskdsv5aU14NbsXL1q1cNxQ7RnOUAmPCsaxJ0meYoXjTdUOj5c49kuB4y6GUKk6aMoMjXQgjUa1zxfFWbkFLAtXJ8WU+AiNgvIzVuv/wDw9tkyLregAI9aXYr2LZBpcDecn74psoTjH5DsflQnJauSrWcOGIA3JgeZp1c4Vbze7Ri5VZuHYKdAyxzg6aUG+Fa20Eag084DibSZrblR7xMs/wAM66RsZ19BSIvX8N/c6rSUdS3KtxXgoS4VDKFM5WaQCQJK6AwSdBPOl9/hxtsVMGNJUyDrEg8xI0PONKvON9kits3BcVpE6iJHnO9ILFpbeZLiZkYCcsZ1iSpRuRE7bHY9Q9SlFKMtvmZXjUrlHcr6YUzKkg9Rp9KsHDOI8QBzW2e7k5FDcgemtA2EKnaSNjG/eKf4W/dJPu/ATqxHh9dKCWVf7GecVFBPDfaDFC4BcwqZ41Yi5agHSWhW0nSSNzW7/tSy4j9pYCIpKuFOYkawVkCOR9aY2+HXgAP8QJOhBViI6TOooDjXBDIJYMMskxrO0SfIUuWWMVwZ3kixtwzFYJ7q3feKoCsSLhy+LTKYb4tz5VYUuqIy3LZB6MsGOleaYTgfvyigGJIbQxEff/0or2k9lrNqw9xQEKFRMwsEgHbzqQyxuvf5C5yUj1S1isyiWWD0Onzoq04gQc1fPQuWVTKi57nVpCDyB+I/dUuG4xfVll3P2Qo0gdFiIrWssq2X52YPo2rR9EFRG1QKnirzb2f9sVFsreu3QwOmZWbSOZE/fVmwvtHbuRkvKexEfgKdHIpJN7C3imumWSWrKVf5k3VP161lHsBpZ5LjMZJNBBiTVuxPBrQEgbUHawqHYUemgtZ37NYqzbZjcYK8AJIPPflvRftXejJaDcpYf7jAPfSYrjh1i2t5WcCFBOvWNPzoLHWLly4Qql3YkzyA6k8hWDzMmn4VyxUouc7GPAXz2bts6ka/Mf8Atpfj/A+Zf5WH0P67UTwHBNYuyzTmBUjl1H0j1rOP2ckg7f8A4muVPlNfQKeNxe4Q0nD40CA2QOpO2is679CKotv2odlgojHlGYfnV6xixgrhn47Soe/iCx8ia8/u8OQ7iO40P9624fSaqSCxx2AWx9y44XYswErIOp5VZ8Rg8qrKyxEk9SBJ/Xag+A8ADNcuZiVQQumudgfnAB+dWmzaGJtlkdFNtsjnXQqBsANdDv37UfkTSpR4FZW72KbebSYgGrJ7BMpN4wC8IBIGxzTHyoPiGCUSAZC6THTSe1LeGcSGExKvJK/C4GhAYSNJ1I0NBXqQaSKXxLY9itYWbZ1YdDMR+dJ/abAubD+6vMHVCRBknKJg6c4IrScSLW81q9bZCu8gFfnsfOk9zjt20wAYXpEgaepzgaffXO9SV1ju10/+BR25KrgnLXgrOwLiBmJ1b7IM7Ty7kdaJxFhl3H6/A1YfaQ2rtuxduWWZXJDXFEMg/hkakhpHoYoDj+Lw9wtctPlcfEjAqG5ZgGgzT45XNxdNXs+1t9Df4/myxuugdOL3fdrbLSoIPerTbtYW9ZUMxzLrnBhwZmNRqD0iqJh8SroHkDr50bhmJ1Ex2rT60oWpK+tzsXiyxTUq72HWH4eb5Zf9JCRAAPiOm3lMdWJqmKXsX5YHOjagk+IcxPcV6X7IoVNwncgAzv1Hnz+dVD234S/+Mm2WAe2rQNpBYaA+QqYpanbezOJ5MnPO4xfBFifaFrnhsg2hMmWDsewbKAB6T3phY48biorgkgBbjaQeXLQEgbedLfZj2Xe+7NccratmHIAzM2n7NTGh6nlp1q8cX4WnuhaW2VtIVYi3p4gNDJHibXcmdqLPgisep8dGaUpRlT5NB/dKr2z+zPxRsJ+18965xttcSjWmko0ZiNBOhGU8yOtAYPCAoVD3CgMnMPDt5AGrNwzAgWwRqAR8p1mOlcpOcnpxvf8A58ya2iu/9hLBWLb3FaNzlZfMiAeXIilHEfZG5YClgHVgYZTseQKnYkTEE7fP08yuoAIJA0HL+1ZibYZMp2aQZ3idD510IxlGL1SbpDMPkSjLfdHmfD8GFaArNC+R+kHfqKe4a0iqoNuJPMLMx1mgmtutwqfiB1Eg8hJgkQCBoRXLu+cDIh2nMDsdCVI0Db6eVKjN82dppNbDv/KLf8H3/wB6ygf8Lb/jb5n8qymeqwNHzF3EcUwIUc6h90ba5jzqDEO1wwBtzqf/ADFVtkXT8IMGu/scNIGwF1bl4WiGOhLnYBY6/IetXa1gLdq0Ag31P4a1WfZPCAI9wjRzAY65gBqfU6R2qxY3iSKBMKo5kgD765HmZoan71SN2LE0k0CX8POvOl3HGLKnh1G/SjLfGLTGBcQ+TKaOte5uCHaK48HO64v32HThF7sRYh/eYZU6MJ8gDVav4YlgiAlmMDzNXB8IpZgh8MwO87+kfWinwVq3kKXFV11GYSJ+prVghNu+hEoKK2E7cPuWcL7tYDGWb+ad/IRA6xVe4Ti2wzPFuUeBBMQR0J5akfKrpjeL27h91mBcg7A6kCYjfYHWlI4MXJciFnQbnzLExWjNJJuPKME9SdNCbHF7jNkTImuWRLAGJg7CY7x1qsXuF3EaSM+smZk+eutX1sCgIy6tPI7+Z0mgrmDYySw5n4SBA5A7H0qYM8k6iHCcIrfYK9hsAj2CzJDG40yDsAsb8qftwhTJAAJ59hsKz2fwvu7IDQCWLfOAPuApk+KUDeuR5uWTytrZsmzbYJhOFNbBy3XAP2fiXXU+FtPWK0/CJYv7wgN8S5LZVh3GT+9H27ykArqZjppQftJxJbFnOgBeQuuo13MUnG80u1b2Dgk2khD7R8HQp7q0lsFgSzZTKjtB308tO9J+C21w1t0xAuSXzoVBaRlClY2GonWN6ccL4sjg5ozSTm116z31Pyo3/E27gjOv8MHckdvxrqYk1j9OTv397Oh/jpR/kM4Hxm1eCrbw19lBI94wtqs+eeT6Cp/aHg1zEKuW2mZToSSdPtAiPF5SOxFVa/7O3Evo2HutbzSbrK0ZANoiJJ0EH86u/AEupbAu3/emT4iFU5fsg5ecV1cWLG4pUYMmP05akyLgXCiiBcpUJoO/fTTMTJnvTriDC3aYx4ogdydqOVBEmkfGuIKBq6gcpI19Kb5WWOHE/fhGfeTsScO/Z/GAQxIMa7/2p7ZstbTwmREgHpJJ1HpSTBcXsuCHzdvA+usTt9ad4DG23EK+2wMqfQNr0rieNFJtvb26YUsU0rphHv5UP0mRttFdMCfSoLSeJwxGU7Aemn0otDoQR/cHStkbmnf9ooTcZ4Sl0LcA/aJzmMyiTlJ5byDyqrPjbloqjgAMJ1ysRoQSDpqOh++r4++WZ8941pJ7S8EXEWnQSLiS9sjeY+EzuG2PmOlKfNcb0a/H8hw+GW6K9/m9v+L6VlUr/LU/1D+vWt070f8A1+xu9WPsWEHnNC8Zj3ZKiTzHUdR1qC3dzEAkxReLAcr0GkV2b2OUtmML/HUW1bt2QJ93PKFAA5HcyfrVHu4e5cYtdZ5PNifn2125Uya2ilh4lkjI0mI5giPSh8ReM+8BzJoBMaHbKVrKsEIu13+TTrb5FuIwFxNJJ2IzbRyM+taPEr9owXZWGoEyCO1WG9iw9tNs8H3mn8wIEAwBAUelBYnBqyBmIENAkbDeTEnXy3q2ot1JWiqfTOsBx29cyKz5SZ1B6aid4mnWKBDNnZicg3BMyZMclIgnXWKrGDtsXdEgQGfMZmFkkAjy+tOOHX3Um3mOc6ak5RoMhA211iqWKMd4rYtSb2bNNibtu4DacLoQpUTyg5t5E9etd4zjWJfNcaYGyL8IMDSNZM10GuW7gzKpgTlOqlSS0DXUHMw5RFcJjVLw65QWGYgkgaiYXbYmI8taCUIz5VgyiiC1xbGLquQ67FB8tIP39ahfjmIJ1KIfhELpIIJABJ6CouMPcF0+6ViBsACAQAfERyJGs0pTCuzZmlRoYJkz211560SwwXSQp44XwemcHx5uYdHe8rsJDZmVIIOoMnkdu0UHxv2j9zaDobdyXywHnQAknTpAHTWqgMNqAy67idZGusfOj8Fh7baMoKzEnQelc+XgY9euTve6CWLfYf8ADvaYXIzfs2O07eQ5E0zxIvFc63cw5rCn5gjWq5f4XbMCSLesljoGGvOBG5+dR4bH3rKrBzWwIM79JnkD6/krJ4MV8UF9n/BoikuUaxlhgSYyk66CB6DkKgsC4wER4STEx9akxHtRbJyurZdpiQD5TNPfZm2jlbyw1tWjn4m359KkteOGqcQ/VUeGWr2ZwL2rIN395cgsD9kQAE9PqTTC5aXkB1g7VPeeChjwuPkaQe2WJOQWrTFWYZmYGDA+zPc/Sjj5GlVft+5iWrJP6j2/jTfsMLZgmQSDrA3jmJ+hpfg8ItsEZSdDE7SehO29U7hvFruH8MZliNNPUg71ZMH7U2XYIxyHnO2nbcffT1mhlacuV+DV6UoJqO6/cY/4VS2gG+40MfjRVnAIQRBIPLyA5VnvrbQAwlpy+KQ3Mx3g1KcciEAnXYbfT0p6xYuXQtzycKztOHKsFRlIG4Ovl/ahsfxEYa2XuBmQFdVEkBmCyRzAJmpzjwedVP2z4iLiC0rAgEtcjcZQCF8yTP8AtHWhyQxJXHn5C9EpP4iw8Ox9m9cz27gbwwYDCPny/XOj7hAzPBmOZ5dq8r4LnFy1dtaZU8QLQJ18JXYyNPy3q/W+Nq4IIGbcLoQR2P4b1izQUIP25v5lTwuO64DMtr/TT/wrWUo/x7/wfdWVy/8AIl7gFCtoZ1otFPIR3Nd2wB8QoHE8QJaE1HU/lXsG6QSVsO4tetvaW1ABGoYQCG51Ub3D71sOXErAMgiNe2/3c6aXrrsNQPlTQMHZVc6ZRoOfbtWWPwuvdmlrV9io2sUuxI/vUr4owY1H0p7ifZe25ZtQdwonX+UD8exoHG+yNy3AVoLEQszMmABzJmmPSL+IWJdMzETp58/wpiuJy25VgTm8UxMxyO86H7tahv8AAMSigImeR9mY3IP0NCpwHF5f3ZEEzoTqIkGBpEii6K7GDYox8WhA31MiRGumkiO1Jbt9mObbLtR54NiVbW0421IJGvaKXYvDX5+A6D7MH1gbUMYq6Cm3XA8wvFi5thmJgQy/yiGUT/DIHppTIJbKZwsEBROmokBoEdp9apvDXfPojFoj/rO1OPcYvQrauEHopYfdVZNuyQae5YONX7TLbgS+kRyBzBgY7wPUdKCN8MuhOgJI7DU6E+sedKL1rFKxBsu22oRzy2kDfXlXWXEGAMNd/wDLc+Wsa0D+35CTRZMFireUsbjINRp8ShhrAPxAydhOgobHXzecW7fibLGkAFpLDYxP3zFKcRwrFFoWzcgwZCMBrrzGnl50Xa9nsWAgtyrMTmLAoF1/ikz8qVKcF+qS/ITdK6ALXCbmJue7tLncySBoq9ySYjvXqfCOGDD2bdhRIQS3diZY/Oag9j+FLhLeTPmbVmMAAkgAgc400p44liBvEisHkeVHNBxT2ul8zHOVvYJFrNbyycw+Gl/GSjYcuFJa2uY6SYHxDTnFEvxGMnn4u3KK1jsXatMXB8QGZlGq5Y1JI26+lY04y4rpP6fIGMnF2irW7SXVBQgg1EeB5iCVBKnTqKQWuNhLjXIW2rvPu58K5pIg8hsTy8XKKb4f2vVXgpI5kGfTanrw8sXtwdSOZNb8i3jd17V5bdp2UqJbKTrOw+776T3MZeUnMGJPIk9/yPyp3jgHuNimYC2csFPENSZVujb8o/DnHYa2GtXrbm4DoysTIIzQSo1AIJrqY8KjBKS3oW8rb2YNZa+qli3LbMw1PKRqI50Za4bu8EJ7tSM05SzmTGUb5hB3771zxjj6Pca3bhUysWAIGuXxDUawCdO3ageBcQxBFy3bXMoI0Y6Kfs68jpRemlG6pAObk93YbhrvuWyKJYjlvtynTSPrTP2Uw1triMc1w5mDZiAbZXNqQDqQQF82oDA+z9y5czli08pIIGUqQdOpmdKuHs9wm1gMNdeDzLFjmJI2++lz0Tg4p9BJuI6z2v4l+YrKoH+c3ug+VZXN/wAZDdRNxHClhCrl66zPft6UjvYUryNX58GNv199A4jhitpNd+/c56ZRXkcj8q7wVzxrmn4hB9dvpVlv8EPITSnE8Pe2Z92d6CUbQ6GSmMcS5a6jKpy9eUwTuOfL5V1jcWff2y3iFsknXXURttvG1D8OxyrcTPsSV13BI0IHpHrUmOSbt3UDksayYJg/7VJ9Kx3Nf32ND0sYWeJqYW2R4RJDQoJLjWQDsOVRYrGNBBQZSGKrIIzHQEmBpzgR9CEWBsFCSW56eUfn9KNt3sxg6gR+h05/Oj9ed87E9OKBrmMKiFzBi3I6wSDvvMmpkuGW8IKHQAjMQsxE7rJJ1HQUDxJYuIyAkFxPQEEfgPrTu3cAXxal40g7D4R6R9Kt5Vyw0HWuE4S4ELIUYblDEmR15TOlH4fBi2f2d4ZT9lt/mPypA2JOh1gTGvLQRHY1G2L5Hv6VlyZHJU1aLWOnaZcExqjRwPMbfMfjR+Gtpc+E154uKMggnv8AOibWLZY1Op11iRWJwp3yhum1tsy+37FpB4nA8yB9aSYi/bYlUaeelKFugbjvrr99RvisraLr2/Gk5ManwqKeL4Wm7HltuVE2MQTqR4lEjuNopJZx48UzmAnlyG9PcBirTDUiY58p7daXjwy1pXS9znz8WafGxtsOX8R03mIO/flVP4hwLE23LpinVDOVM2aNP5tGWJkGr5bvWjK9P1NdXbdtuhMED1rs48eNL4Wrf3B0uPMTyjEeyrsVAZARuMuTrqFXQegG1QYn2XK6viEBPKCT666V6DjuCo9xQ7wmXrBGx09RNV/G+zyW1IW9tJHhnyBIq/VyRdOX7D4QjLoqKcHcaZ5U8oPzouxwBvD4jrsAdZ9Nt+tPsOmQBnZTyGk/Lv3rd3iKW1YIPEdj011qPypPYZ6KXBHw/wBm7QYF7cROrBiem3wnrNW3CcJQCEIAB6DbtVTwuLu3G8TgRAineGxLoIJEa+dZ8nk091f3CWB9bDlLaWyQognnJP31Ljgty2LQGkgnvBnX11pPbvtcMLuPu8+lOcIhUamep/LtV4HOb4pFZYxgubYD/k6fwfdW6cf7hWVt9NGb1GCkDt8qjYA8vpUeH4hZufBcUnpP4UUAp1BB8jWyjKDMg5CtZdII84mislaIjSP18qiILruBtvo1tWHcA0DifZu07BwWQjocwJg7g7709y9BWNbPOq0JhKbXBUH9lLgMrfVv6lK/QmoU9nMSrTFs6D4X8gdGgbAVdQPL1rQNB6MA1nkUe9wy+GBey0DkBm5g7rP6mocRd1hgwI5EEbefOvQATQHFOJ4e0v7d0A6NBPypcvGT4Y2PkvtFEN7v+ulbD7frypk3HOE3SQMqHqQ1v+1dDhuFua2MUk8gWVx9xmkSwSQ+OeLF6Nzmf0P16UQhBGvI9K7bgGIX4UW53V185OYjWtDhWLETYc+qH6NWeeGfsOjlh7hlvxd/1OvSpRbB8hPzgCg7aXlPisXR/sY/eKMXEodHleoIKmOsHlyrJOE49Doyi+yQ4fTTc6H8fpFTLYg6VDdxltN7ijXbQDSevyrVvEuzRaRnU7MFJUdiY/Ol6JS4QTklyGZIJM/qK0+IjVTEQZ9a2mBvuJZAuggE5oPXTfynlQtj2Rckm5fuNLZoXKm/fU03H4k5c7Cp+RCPZzjseoXMxk9J19ByoLD41WOoGo0G5PaBvViw/svYQ5jbDHmXLOf+YxTO3hbaCFVR/SoH0rVHwn2zO/LXSKdi+GXLpAtpkUHd/D5wNz91cf8AZYkGXGaNDmYgHyjaroQOf0rTOvStEcCSoU88myq4bgl1Nja56+IRpv8ADrrFSpwFnb9pddu1uEHzkt94qxe9QztpvqNPOulxlsrIdcsTIiI11kctD8jRR8eN2DLyJkOFwS21AAAHTv36nuanVidhNDf5lh2H75SOxPPTSB2PyPSsX2hwqiBcUAfyvHWSY56U5YkIc5MM92etZQ3+fYf/AFP+R/8A9ayi0IHUyg3ry5DatrAMkkmWbuxGvkg9eg4E2hGczJlAYy/1EfD/AEjUUTatggi2pyj7cw7ach9lf5jBgVJhxh7Z0UO4AgqSVUmdj9ozHfpWiiWcWrtwEXHuOBp4VbVh/KpPhURuaJt+0F220s+a2IBzL81Ug+I99R5RqpxeJJY5gWuaiOQkzrH0HTflUVuw7sYIJEZmJ8CjoBtp02qUiF0wPtbZuQGVrZbrqNdtthTMcUsGYu2zG/iEa7a154bK8pKTBeJe4SNVUHafwknYVE0CQAggyFJlLY6n/Uf9eVUSkemm8kTnWN5kUox/tNh7Q0Y3DyCCZPQHaqHcQHQlyx2UmS411b+Fef6muXeGlTmeB4gNFgfCnSB9r5dahFFDbiftZiLgypFqeS6sPMn7XYVVcRhy5zMSzHmTJ+Z5/Sjogzp6fhP3tXS29Ntx+h2XvzqB0hO/DwdN+/XsO3eojwwEwB6j747d6fph5/X07VJbsz4eR3PXXby7c6qy9KFGHwV1RKXLi9Idh+hR7XMYqS2KuhY08Rk7U9s2AJL8pkaSO396UcTxPvG20Gw5ChbthJITtjsWDpibo/3t+dWXgY4gwQ/4u6PeaqCQ0IIl2zAxMgKOczsa54FwhX/bXVJtKfCsa3HGygc1mAep061dERhC6C7c+Mrr7tB/Dp3gdyT1qS44BtWD4TGXkZnZ0e2ggu1tS7NOylQNj4ecknpqU3EMVlVSyC68mMoIRd9TOsDSebHpUBv2wvvAJtWiVtKPtuDkzd4nKvfMddDUQuhveAnMcoe8yzouuW0n8U7eWc7mkaGHaO7/ABq9ujrBBylgNQNDdaBIQTpAljEaQGiTF4x972TSScijKupzPIME8kGsbmQansYcuztALK4QAbG6QNP6banTvJ3qZMqxALw5RAdM9z7V1p5DoOhgaLRxgwJSSEl25iS62xfusWJ6qzAjwwAoCc5kiBuQTTrDYV7ZzXLrPdKjJb95oo0BbxGDrEsdBsOZMti3Hhtz7zQXLjAM7ZpYW0zmJIkwdFGpnmY+FGRzoP4m5eE6gudXOkdOWlO0C3KxMllyXNy4AjEF3BKyP9JSdVUDTSD4mJObRRseWkuMoY2ywY+BbdoMfdrvIY6eE7mdfCI3xLi+XLbFiDyJVR4VOhKiW0kGNDrtNKsdZuBVNzMGuSH1jNGYyQdAq5oURprOtTQWrB+HgXGAKqFRWJ9370aasWYqTJ02+mhE2Nx21u2pyqoChghJgkalNoGmsyszvUeIxDmyiLbOTPGaTD3CFkZVAV4jTNJ1PemODwLMtoEAtnIdiM1xVUwVW2JYiSxLEcgIAolApsDThxzp7xjLkuz6Flt20lmA0KHMwVSY+yY2FFYbB5fFo1thsC2QXCSFWHEMFkwG6zzkk4R2z3cRlFy3dzW7agkAomrqPBKrCyDAmddTIhtXgrq1tpW7clgzEhTKEgiAFc+X2tztRKFgykSe6b/SX/k//jWVZ/d3f9P/ANP51uj9IXrRTMTiRkITRT8RIgt/UeY3OUUC1smCPDbEeLqenbyFO2wNssB4icvhQaqo71tMGgBg526bIvcVbgWpihcPkQFpAPLQs3TyFRXVLaTAH2eQ13Yjc0yfDSczXCFGmurOf4UHLzrBhlHxQqjXJyHdjzPah0sOxRbtGNJAOmcDxN2UfZXvUF2BtEjaNk/Nu9OHthhIJAOgH2n8hyFDhAsgIC2mXmB5D7TVWkIVMxjn36nuTuB2rSWiPX9fLtTF8NlOu/Mbx27mu0tRG2mpnZO56t2qtJdi9MOSdtf1qeg7VPawLN1gnc8459l70ww9rMdFOTck7t/M3btRN9jEKYn/AJh1jkO1VpJYsXDhmyqfCD4jtMcvLsKb4LhswANtWPJP/dHLlXeCsE+BR4uTEfD386441xMW0Ni1/vYczzoWi07FnGsQuYpb+EHU82PWoeCcGbE3FWCLc+NugiSJ6/nWcM4e+JuC2nmzclHXzr0TBYVLFqEEKogdWPM9yTVxh2ypzrZC5sKnvM65USwkCFLAEweXRR/zVDfufs0gtnxLgBwCIQnry8HLue9ObyOLQQGGff13rVxVzIo2tGexYggD76JoBMXY+wff2ragBLasQABoYCqY9TUPDUHu1YnxXMV4yREqjGBHIeACBRdt1zXbhnmPRd49a3hlyLbU7qrXG/qM/mflVUXexxwhxltOc0vibrHqSA4BPaFGg7VFw686+5gErcxFyQwG2ZyDJErqAY7VPwyyQMOIIMu55bgz/wCqibODUqjg7YgtpsviMj9daYo7AOSOsNi2FyCgJOJI6zFmGYyBERReDv8AvrboVGUPcTf4oYidOczQ97CFbjFSV/aC4OYMpkf9dqFxN3FWZt2lVlOZgzRuTJAqtybE2GDo5BJuLnK5iq5gCASpO5gkQdfuqpcVf3eNM2wUN1CyR4WGw020Jnz3pwnD8c3ja5a1bN8MkHaQeWlQ4nCqoW5cJZ7TjL4hlYcyRGlGo2TUkAcOwxZ7qJc91duXDlaBPu/FKodAhJABiDpW7mMv4XJbW1BJIEhgSM0/ExPPvTjhWFtXLbnRiXJCsVMEmdPI7Uk4xgbltSWZmlsoUnMABz1nLrtUlivcuOTdogtpduOXdABcIhYZiBzYFd9oy85jSmuNtKzlUQWrchs1weNwAFFtd4gA6trr2Fc4TG2j47tz9ooidMn9IUbaAetT8MxGdmtq+YvJKgCVJ3YE7ACmQgooVKTe7G3+Y2v4rX/m/wBqygv+xtn+K7/4h+VbotgdK9wTCf8AeeR+lL8L+6H65isrKBlo1iv3q/00Hi/3f+/8aysoX2MQbh/33/06E4d+8XyasrKENHD/ABj1rn/uh/xPxrKyqLQxT93c9KjP7wVlZU6J2OuHfDc8vwqkX/ibzrKylPkOHBbPYL93d8/wFWa58CeYrKymiZfqZu/8afrrQa73P+J+FZWUJaF7fubn9LfWp8Vu/wDwRWVlWi2Hp8WH/pP0rML/APL3P+M//wBw1lZRiRhiviteX4VDjv3aedZWVAkQ4/8AdD1+hquYn4T/AEGsrKZEEg4F8Tf7ace0H7h/MfWsrKMH/YqGB/eHyp/7L/vLn9J+orKyp0FItVZWVlLAP//Z" height="110"/>
          </div>
        </div>
      </div>
    </div>
    <br>
    <div class="row">
     
     <div class="col " style="background-color: #faf6bc;">
     
       <div class="d-flex justify-content-between">
         <div class="p-4">
           <input type="checkbox" @change="GetTotal(shawerma)"/>
         </div>
         <div class="p-4">
           <h4>{{shawerma}}</h4>
         </div>
         <div class="p-4">
           <h4 style="font-family:Cairo">شاورما</h4>
         </div>
          <div class="d-flex">
           <img  alt="avatar image" class="rounded-circle"  src="data:image/jpeg;base64,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" height="110"/>
         </div>
       </div>
     </div>
   </div>
   <br>
   <div class="row">
     
     <div class="col " style="background-color: #faf6bc;">
     
       <div class="d-flex justify-content-between">
         <div class="p-4">
           <input type="checkbox" @change="GetTotal(taamiya)"/>
         </div>
         <div class="p-4">
           <h4>{{taamiya}}</h4>
         </div>
         <div class="p-4">
           <h4 style="font-family:Cairo">طعمية</h4>
         </div>
          <div class="d-flex">
           <img  alt="avatar image" class="rounded-circle"  src="https://kitchen.sayidaty.net/uploads/small/f4/f4ea3e276680b00312d6fa9f579c5ef4_w750_h750.jpg" height="110"/>
         </div>
       </div>
     </div>
   </div>
   <br>
   <div class="row">
     <div class="col">
      <div class="alert alert-success text-center"><h4 style="font-family:Cairo">المشروبات </h4></div>
     </div> 
    </div>   
    
    <div class="row">
     
     <div class="col " style="background-color: #faf6bc;">
     
       <div class="d-flex justify-content-between">
         <div class="p-4">
           <input type="checkbox" @change="GetTotal(Fruits)"/>
         </div>
         <div class="p-4">
           <h4>{{Fruits}}</h4>
         </div>
         <div class="p-4">
           <h4 style="font-family:Cairo">كوكتيل فواكة</h4>
         </div>
          <div class="d-flex">
           <img  alt="avatar image" class="rounded-circle"  src="https://kitchen.sayidaty.net/uploads/small/6d/6d8706af3cc27a0c0e7666e4c5c1f861_w750_h750.jpg" height="110"/>
         </div>
       </div>
     </div>
   </div>
   <br>
   <div class="row">
    
    <div class="col " style="background-color: #faf6bc;">
    
      <div class="d-flex justify-content-between">
        <div class="p-4">
          <input type="checkbox" @change="GetTotal(Pepsi)"/>
        </div>
        <div class="p-4">
          <h4>{{Pepsi}}</h4>
        </div>
        <div class="p-4">
          <h4 style="font-family:Cairo">بيبسي</h4>
        </div>
         <div class="d-flex">
          <img  alt="avatar image" class="rounded-circle"  src="https://tomtom.com.sa/media/catalog/product/cache/202feff92cd010e93148dbe3117b7b41/p/e/pespsi_2.jpg" height="110"/>
        </div>
      </div>
    </div>
  </div>
  <br>
  <div class="row">
    
    <div class="col " style="background-color: #faf6bc;">
    
      <div class="d-flex justify-content-between">
        <div class="p-4">
          <input type="checkbox" @change="GetTotal(Mirinda)"/>
        </div>
        <div class="p-4">
          <h4>{{Mirinda}}</h4>
        </div>
        <div class="p-4">
          <h4 style="font-family:Cairo">ميرندا</h4>
        </div>
         <div class="d-flex">
          <img  alt="avatar image" class="rounded-circle"  src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTJlCQeDchi8M4qV3CbshemeMOFZYNOvQn24Q&usqp=CAU" height="110"/>
        </div>
      </div>
    </div>
  </div>
  <br>
  <div class="row">
    
    <div class="col " style="background-color: #faf6bc;">
    
      <div class="d-flex justify-content-between">
        <div class="p-4">
          <input type="checkbox" @change="GetTotal(water)"/>
        </div>
        <div class="p-4">
          <h4>{{water}}</h4>
        </div>
        <div class="p-4">
          <h4 style="font-family:Cairo">ماء</h4>
        </div>
         <div class="d-flex">
          <img  alt="avatar image" class="rounded-circle"  src="https://cdn.salla.sa/ZPdPZ/BWSHFUxinBwJ95eHmiQlkF43Hb3ZZ4U4zM9G4T1k.jpg" height="110"/>
        </div>
      </div>
    </div>
  </div>
  
  
  
  </div>
  <footer style="background-color: #c7d9e9;">
      <div class="container p-4">
        <div class="row">
          <div class="col-lg-3 col-md-6 mb-4">
            <h5 class="mb-3" style="color: #0a0a0a;">توصيل اونلاين</h5>
            <ul class="list-unstyled mb-0">
              <li class="mb-1">
                <a href="#!" style="color:  #131212;">الاسئلة الشائعة</a>
              </li>
              <li class="mb-1">
                <a href="#!" style="color:  #131212;">التوصيل</a>
              </li>
              <li>
                <a href="#!" style="color:  #131212;">المناطق المتاحة للتوصيل?</a>
              </li>
            </ul>
          </div>
          <div class="col-lg-3 col-md-6 mb-4">
            <h5 class="mb-3" style=" color: #0a0a0a;">قائمة الضيافة </h5>
            <ul class="list-unstyled mb-0">
              <li class="mb-1">
                <a href="#!" style="color:  #131212;">الاسئلة الشائعة</a>
              </li>
              <li class="mb-1">
                <a href="#!" style="color:  #131212;">التوصيل والدفع</a>
              </li>
              <li>
                <a href="#!" style="color:  #131212;">قوانين الارجاع</a>
              </li>
            </ul>
          </div>
          <div class="col-lg-3 col-md-6 mb-4">
            <h5 class="mb-3" style="color: #0a0a0a;">الشركة</h5>
            <ul class="list-unstyled mb-0">
              <li class="mb-1">
                <a href="#!" style="color: #1f1b1b;"> العنوان</a>
              </li>
              <li class="mb-1">
                <a href="#!" style="color: #181717;">رقم الهاتف</a>
              </li>
              <li class="mb-1">
                <a href="#!" style="color: #0c0c0c;">البريد الالكتروني</a>
              </li>
              <li>
                <a href="#!" style="color: #131212;">تواصل معنا</a>
              </li>
            </ul>
          </div>
          <div class="col-lg-3 col-md-6 mb-4">
            <h5 class="mb-3" style="color: #0a0a0a;">شركائنا</h5>
            <ul class="list-unstyled mb-0">
              <li class="mb-1">
                <a href="#!" style="color:  #131212;">التسجيل</a>
              </li>
              <li class="mb-1">
                <a href="#!" style="color:  #131212;">التطبيق</a>
              </li>
              <li>
                <a href="#!" style="color:  #131212;">القوانين</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="text-center p-3" style="background-color: rgba(0, 0, 0, 0.2);">
        © 2020 Copyright:
        <a class="text-dark" href="https://mdbootstrap.com/">سلطانه.com</a>
      </div>
      <!-- Copyright -->
    </footer>
</div>
  </template>
  
  <script>
  
  export default{
  
    data:()=>({
    Borger:30,
    shawerma:10,
    taamiya:5,
    Fruits:5,
    Pepsi:3,
    Mirinda:3,
    water:2,
    total:0,
      
    }),
    mounted()
    {
       
           
    },
    
    created()
    {
      
     
    },
  
    methods:{
    
     GetTotal(n)
     {
      this.total+=n;
     },
    
          
    }
  
  }
  
  </script>
