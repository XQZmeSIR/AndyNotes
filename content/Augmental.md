# Augmental

The Augmental folks kindly invited me to visit their SF lab on [[2022-08-23]]. I was connected to them through my comments on TouchBoard, a [[Silent speech interface]] in the form factor of a dental retainer. They’re working on an input device in that form factor, currently targeting customers with motor disabilities.

Their device fits over the upper molars. The form factor has a very low profile, so that it doesn’t impede speech. It has a small touchpad surface, meant to be controlled by the tongue. The touchpad can sense pressure (for “clicks”, like a MacBook trackpad). The device also contains a 6-axis gyro/accelerometer package, and a temperature sensor, as well as some mechanism for detecting exhalation/inhalation. They intend—but I believe haven’t yet included—force sensors on the molars. One early prototype featured a microphone, but there are evidently some considerable miniaturization and power considerations.

Perhaps because I was anchored on silent speech, I was initially underwhelmed. Sure, maybe you can cram all that stuff into a retainer, but can one _do_ anything useful with it? A startling demo made me suddenly pay much more attention: co-founder Tomás put one of the devices on, connected via Bluetooth to his Mac, and used it to move his cursor to the tiny “close” button at the upper-left hand corner of the front-most window. He “clicked” by pressing with his tongue against the trackpad, and the window closed. I was very impressed—that’s a tiny hit target! He hit it quickly, on the first try, and with no visible motion of his body.

OK, so within certain parameters, this satisfies some of the characteristics of a [[Poor man’s brain-computer interface]]: it offers omnipresent, hands-free, screen-free, invisible, multi-axis input. That’s worth taking seriously.

I wanted to be helpful, so I steered our conversation towards interface design. I suggested we spend a while riffing on mass-market consumer applications of this device. A framework I found generative: as a persistent, unobtrusive device, AirPods are the mainstream modality to beat. For discrete, command-and-control input, they’re great. Their significant deficit is that they’re not fully unobtrusive/silent, and they can’t really do continuous, multi-axis, analog input (except dictation, which counts in limited contexts). So, focus on those elements. What if you had something “worn” like an AirPod but which could produce output like a trackpad?

A few directions I particularly liked:

  * In my recent survey, my favorite [[Silent speech interface]] modality was [[Fukumoto, M. (2018). SilentVoice: Unnoticeable Voice Input by Ingressive Speech. Proceedings of the 31st Annual ACM Symposium on User Interface Software and Technology, 237–246]]. But one problem with that approach was the form factor: in Fukumoto’s system, you had to hold a pen or ring up to your lips to speak. I think there’s a good chance you could use Fukumoto’s technique with a dental retainer modality like Augmental’s. Then you could wear it unobtrusively all day, and get SilentVoice-style silent speech, hands-free.
  * I get excited about this for omnipresent AR/VR systems, worn continuously throughout the day. I expect at least some people will be adopting those by 2030. These systems desperately need better input devices.
    * The grip controllers work fine for deliberate sessions, but for impromptu interactions—or when walking around the city—you don’t want your hands occupied like that.
    * The AR/VR manufacturers are emphasizing hand tracking, but [[like Bret]], I’m pessimistic about waving-hands-in-the-air interfaces for more than the briefest interactions.
    * A retainer-based input device would offer persistent unobtrusive input. Many VR/AR visionaries imagine that we’ll “always” be playing a game as we walk around the world. This device could offer a 2D joystick plus 6-axis head tracking. Not a bad game controller.
  * Electronic musicians are going to have a field day. Hands occupied on an instrument? No problem. Foot pedals are 1D; this thing’s got 2D input plus 6-axis gyro/accel.

## Data

  * Co-founder: [[Tomás Vega]], formerly of [[Pattie Maes]]’s group at [[MIT Media Lab]]
  * Co-founder: [[Corten Singer]]
  * <https://augmental.tech>
  * Operating on only a pre-seed round.
  * Invited to visit by Julian Castellón Odabachian, a friend of [[Mackenzie Dion]], by way of my article on [[Silent speech interface]].
