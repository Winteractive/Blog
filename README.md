# Random code
This is a test example for our blog.

```cs
public class Progress : MonoBehaviour
{
    
    #region Variables
    public enum ProgressionStates { NewGame, Continue };
    public ProgressionStates currentState;

    public const string PROGRESS_SAVE_CODE = "PROGRESS";
    #endregion

    #region Singleton

    public static Progress INSTANCE;

    void Awake()
    {
        if (INSTANCE == null)
        {
            INSTANCE = this;
        }
        else
        {
            if (INSTANCE != this)
            {
                Destroy(this.gameObject);
            }
        }

    }

    #endregion
}
```
<p align="center"> 
  <a href="https://discord.gg/tRP76Br">
    <img width="200" height="85" src="https://i.imgur.com/5IA5LTS.png">
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="https://www.patreon.com/">
    <img width="200" height="85" src="https://i.imgur.com/IVthDSJ.png">
  </a>
</p>
